---
layout: left
---

# Custom Problems with `check50` and `submit50`

## Background

`submit50` is CS50's tool for submitting problems. Each CS50 student, upon logging into CS50.me, is given a private GitHub repository in the `submit50` organization where all of that student's submissions will be stored. Each problem that a student submits gets its own branch in their `submit50` repository.

`check50` is CS50's tool for evaluating the correctness of students' code. When `check50` is run, student's code is tested against a series of prewritten "checks" that determine whether the student's code behaves as expected.

`check50` and `submit50` determine which checks to run and which files to submit based on the contents of a separate GitHub repository. By default, `check50` and `submit50` will use CS50's own `cs50/checks` repository to make such decisions.

When a student runs a command like:

```
$ check50 cs50/2017/ap/hello
```

`check50` looks for the path `cs50/2017/ap/hello` in the `cs50/checks` [repository](https://github.com/cs50/checks) repository to determine which checks to run. Students can override the repository that `check50` and `submit50` should look at by appending `@username/repo_name` to the end of the slug.

So when a student runs a command like:

```
$ check50 problem_name@teacher50/checks
```

`check50` will look for the directory `problem_name` in a repository called `teacher50/checks` to find check code. Likewise, students can submit problems via:

```
$ submit50 problem_name@teacher50/checks
```

The below steps will walk you through the process of setting up your own `checks` repository. If ever unclear as to how something should look, feel free to model your repository off of CS50's [own checks repository](https://github.com/cs50/checks), or reach out to CS50's staff with any questions.

## Step 1: Create a `checks` repository

Once logged into GitHub, [create a new repository](https://github.com/new). We recommend naming the repository `checks` for consistency with our own checks repository, but you can name it whatever you wish. Be sure that the repository is public, otherwise `check50` and `submit50` won't be able to recognize it.

## Step 2: Create directories for problems

For each problem you want checked, you'll need to create a directory (folder) for each problem. You can place all problem directories in the root of the repository, or you can organize the problem directories in a nested hierarchy.

Within each problem directory, create a `submit50` directory and a `check50` directory.

## Step 3: Specify which files to collect during submission

Inside of the `submit50` directory, add a single file, called `exclude`. The `exclude` file will determine which files you want collected when a student submits this problem.

Each line of the `exclude` fille represents a file (or files) that should not be collected. If a line begins with a `!`, it represents a file that should be collected. And if a line begins with a `#`, it means that the submission should not be allowed unless the file is present.

The following is a sample `exclude` file from the `greedy` assignment:

```
*
!greedy.c
#greedy.c
```

The first line (`*`) signifies that all files should by default be excluded from submission. The second line (`!greedy.c`) means that the file `greedy.c` should be included in submission. And the third line (`#greedy.c`) means that the student will not be permitted to submit this assignment unless `greedy.c` is present.

At this point in time, if you push your changes to GitHub, students will be able to submit your custom problem. If you want to write custom `check50` tests for the problem, see the next step.

## Step 4: Add an `__init__.py` file with the required checks

When `check50` tries to run tests for a program, it will look for an `__init__.py` file in  the `check50` directory of the program's directory in the `checks` repository.

Here's a sample `__init__.py` file which defines three checks:

```
from check50 import *

class Greedy(Checks):

	@check()
	def exists(self):
		"""greedy.c exists"""
		self.require("greedy.c")

	@check("exists")
	def compiles(self):
		"""greedy.c compiles"""
		self.spawn("clang -o greedy greedy.c -lcs50 -lm").exit(0)

	@check("compiles")
	def test_41_cents(self):
		"""input of 0.41 yields output of 4"""
		self.spawn("./greedy").stdin("0.41").stdout("4\n", "4\n").exit(0)
```

We'll look at this `__init__.py` file one line at a time to understand what's happening at each step.

```
from check50 import *
```

This line imports the classes and functions necessary to write a `check50` check class.

```
class Greedy(Checks):
```

`check50` will look for a subclass of `Checks` when determining which checks to run. This new class can be called anything-- but conventionally we name the class after the name of the problem (in this case `Greedy`).

```
@check()
```

Within your check class, each check that you wish to run on students' code is a Python function.

Above each check function should be this line, the `@check` "decorator". The `@check` decorator tells `check50` that the below function is a check that should be run.

For a check that should run no matter what, nothing should be in the parentheses after the word `check`. We'll see in later checks how we can conditionally run checks only if previous checks passed.

```
def exists(self):
```

This line defines the Python function that contains the code for this check. The name of this function is arbitrary, students who use `check50` will never see this function name, so just name it something descriptive that will make sense to you later.

```
"""greedy.c exists"""
```

This line is a "docstring," enclosed with triple quotation marks, and defines a description of what is being tested in this check. This description will appear in the output of `check50` alongside the smiley and frowny faces indicating whether the check passed or failed.

```
self.require("greedy.c")
```

Here, we call the `require` method of the `Checks` class, which is a prewritten method that asserts that a particular file (or files) exist. In other words, the semantics of this line is "Check that `greedy.c` exists in what the student submitted. If it doesn't exist, then raise an error and cause this check to fail. Otherwise, keep going."

If `check50` reaches the end of a function and no error has been raised, `check50` assumes that the check should pass. So in this case, if `greedy.c` doesn't exist, then `require` will raise an error and cause this check to fail. Otherwise, if `greedy.c` does exist, `require` doesn't raise an error, `check50` reaches the end of the function, and the check passes.

The `require` method is just one of several methods that are defined as part of the check50 API. The full API is described in more detail later in this document.

```
@check("exists")
```

Here, we begin a new (second) check to run, again using the `@check` decorator to indicate that the following function is a check that `check50` should run. However, unlike the previous example, where no arguments were passed into `@check`, here we pass in `"exists"` as the argument to `@check`. This creates a "check dependency": this current check will not run unless the `"exists"` check (i.e. the check associated with the function called `exists`) passes.

As an additional note, if the `exists` had made any changes to files or created any files, those files would be copied over into the working directory where this new check runs. We'll see an example of that later.

```
def compiles(self):
	"""greedy.c compiles"""
```

Here, we define the second check that will run. Again, it's a method whose docstring (`greedy.c compiles`) describes what will be tested.

```
self.spawn("clang -o greedy greedy.c -lcs50 -lm").exit(0)
```

This is the contents of the check. We first call upon the `spawn` method, which is part of the `check50` API and serves the purpose of running a command. In this case, we're running the `clang` command to compile the `greedy.c` file.

The command is followed by chaining `.exit(0)`, another part of the `check50` API, which asserts that the exit status of the `spawn`ed command is `0`. If `clang` exits with some other exit status (in other words, doesn't compile), then `.exit(0)` will raise an error and will cause the check to fail. Otherwise, the check passes.

```
@check("compiles")
def test_41_cents(self):
	"""input of 0.41 yields output of 4"""
```

This is the third (and final) check defined in this check class. It begins with the `@check` decorator, this time passing in the argument `"compiles"` to mean "do not run this check unless the `compiles` check passed first." It also means that whatever files the `compiles` check created (in this case, the compiled binary file `greedy`) will be present at the beginning of this third check.

```
self.spawn("./greedy").stdin("0.41").stdout("4\n", "4\n").exit(0)
```

Here, we use the `spawn` method to start the `greedy` program. Then, the `stdin` method allows us to pass standard input into the program (in this case, simulating a user typing in `0.41` into the program).

Then, the `stdout` call checks to make sure the output of the program is correct. The `stdout` function takes two arguments: the first defines what the output should be (specifically as a regular expression, which allows for multiple correct outputs), and the second defines a human-friendly version of the expected output which will be displayed to the student if they did not match the expected output. In simple cases, such as the above where the expected output is `4\n`, the expected output and the human-friendly version of the output are the same. If the output does not match `4\n`, an error is raised and the check fials.

Finally, the check asserts that the exit status of the program is `0`. If it's not, the check will fail.

## `check50` API Quick Reference

See attached document.

## Questions?


If you have any questions about any of the above steps, don't hesitate to reach out to Brian at [brian@cs50.harvard.edu](mailto:brian@cs50.harvard.edu).
