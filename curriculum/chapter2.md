# Chapter 2: Putting the Blocks Together 
(Completion Time: 5 Weeks)

## Central Focus
Students dive deeper into abstraction and the efficiencies they provide. Students will become more familiar with the CS50 IDE and resources available to them within the IDE.

---

## a. Compiling
_Look behind the curtain of make so students get a better understanding of the underlying compiler, clang, and the usefulness of having a program like make to abstract away creating that mashup of 0s and 1s, possibly linking together your code with the code of others._

### How to Launch the Lesson:
Explain the role of a compiler to students. Have them work in small groups to discuss metaphors for the role of a compiler. An example could be explaining that compilers are similar to translators. When two people who don?t communicate in the same language, they need a translator so that they can speak to one another. Students should be able to defend their own metaphors to other groups or the class at large.

#### Demo: Compilation Simulation
Breaking down a simple program like Rob does in the short video is a good illustration of what happens at every step of the way with the compilation process.

---

## b. Functions
_Introduce students to the simplification and elegance that functions provide us with. Discuss how to declare, define, and call functions and ways to modify them by way of parameters. (Note: This is a very important topic and might be worthwhile to spend about a week's time of class here.)_

### How to Launch the Lesson:
Have small groups of students come up with some sample inputs and outputs and have them switch amongst themselves. Can the other group(s) figure out the function based on the samples given? Explain how functions are often a black box of sorts. We don't need to always know how they work but we do need to know what it will output when given a specific input.

#### Demo: Student Functions

Have students play the role of various functions, using pieces of paper as the "variables" they pass back and forth, to illustrate the notion of parameters, return values, and scope.

##### Materials:
Papers to write variables
 
#### Activity: IDE Errors
Have students experiment with writing functions without declaring them and trying to compile their program, just to become familiar with some of the compiler errors that might get thrown.

##### Materials:
1. Devices for using the IDE
2. Feel free to use any of the source code on [cs50.tv](https://cs50.tv) such as [function 0](http://cdn.cs50.net/2014/fall/lectures/2/m/src2m/function-0.c) or [function 1](http://cdn.cs50.net/2014/fall/lectures/2/m/src2m/function-1.c)

---

## c. Arrays and Strings
_Arrays hold values of the same type at contiguous memory locations. In particular, the use of arrays allows us to create "groups" of variables without naming each, but still allowing us to individually index into the elements of the array. (Note: CS50 AP and C are 0 indexed, however College Board's AP Exam is 1 indexed)_

### How to Launch the Lesson:
Have students make predictions about how they would expect a computer to store data of the same type that is related. Would they want this data in multiple places or in one place? Would you want to have access to any piece at any given time or only one data point at a time while iterating through the each item? Have we already seen examples of this (i.e. strings)? Have students think-pair-share their responses.

#### Activity: Multiplication Arrays
Use arrays to define a multiplication table, to give some exposure to multi-dimensional arrays. Have students the index for answer to a given multiplication answer such as 3*4 = table(4)(5) =12. (Note: arrays in C are 0 indexed)

#### Activity: Game Mode
Have students draw out and play games they are already familiar with in the context of arrays. Some games include battleship, tic tac toe, and wheel of fortune. All of the games mentioned above can help students better visualize how data is stored in an array.

##### Materials:
Paper and pen or whiteboards

---

## d. Command-Line Interaction
_Look into ways we can collect input from the user before the program starts running, perhaps allowing the program to take different paths through the code depending on what the user provided at the command line._

### How to Launch the Lesson:
Is it better to get input from a user before the program runs or during? Break students up into two groups and have each defend a side. Might there be different scenarios where one might be more useful than the other.

#### Demo: Mastering the Command Line
The good news here is that this topic tends to be among the least complicated, we've found, in CS50. Writing a few simple programs tends to go quite a long way. To that end, please feel free to use any of the below or others you find on [cs50.tv](https://cs50.tv):

1. [hello 3](http://cdn.cs50.net/2014/fall/lectures/3/m/src3m/hello-3.c)
2. [argv 0](http://cdn.cs50.net/2014/fall/lectures/3/m/src3m/argv-0.c)
3. [argv 1](http://cdn.cs50.net/2014/fall/lectures/3/m/src3m/argv-1.c)
4. [argv 2](http://cdn.cs50.net/2014/fall/lectures/3/m/src3m/argv-2.c)

---

## e. Exit Codes
_Discuss the meanings of return 0; or return 1; and touch on why and how we might use them as programmers._

### How to Launch the Lesson:
Have students review return values from functions unit. In small groups have them discuss when one might want to exit a program. How would your program know how to exit? Would you want your program to always return the same value when it exits or would you want different values?

---

## f. Libraries
_Show students the importance of using libraries and making use of the work that others before us have done and allowing us to spring forth from there._

### How to Launch the Lesson:
Ask students to create instructions to build something like a paper airplane or the like. Specify in their instructions that they are not allowed to use abstractions such as _triangle_, _square_, or _fold_. How tedious is this process to describe the same function repeatedly. Would it be easier if you were provided with some functions that the user already knew such as _fold_ or _right angle_.

#### Activity: Exploring the IDE
Encourage students to poke around their IDE to have a look at the contents of the C standard library files, so they know what functions they have available to them. Knowledge is power!

To do this, students must first ```cd /usr/include```.

Then, they may type less ```<header file>```, e.g. less ```stdio.h``` or less ```cs50.h```, they can then scroll up and down in the terminal window to see the contents. So as to prevent accidental overwrites, the header files cannot be opened in Ace.

Type ```q``` to exit the less command and return to the terminal prompt. To return to their workspaces, students can type ```cd ~/workspace```. It could also be useful for students to search the internet for other useful libraries that are not built into C or CS50 IDE, and identify the context in which one might wish to use functions from those libraries.

---

## g. Typecasting
_C gives us the ability to cast (temporarily change) one data type into another with the same or less precision (e.g. we can cast a double to a float, but not vice versa), which might be more efficient from a design standpoint. Examine the mechanism and some use cases for typecasting._

### How to Launch the Lesson:
Review data types. Have students brainstorm as many scenarios as they can in which you would have a user input data in one type but want it in a different type later in the program.

---

## h. Bugs and Debugging
_Explore different kinds of bugs, the real-world implications of buggy code, and techniques for rooting out bugs in our programs using certain tools built into CS50 IDE, in particular a popular command-line (and, in CS50 IDE, graphical) program called GDB._

### How to Launch the Lesson:
Pair students and have them share the strategies they have been using to debug their own programs. Switch students and have them share in different pairs. Are there similarities? Differences? Are there some methods that are more effective and more efficient than others?

#### Demo: Exterminating Bugs
One of the best things to do here, honestly, is to find buggy code on the internet. There are tons and tons of websites hosting deliberately buggy C code for exercises involving "spot the bug," and it's a great way to fill a class period. 

Similarly many quiz questions available on [quizbank.cs50.net](https://quizbank.cs50.net) contain deliberately buggy code and challenge students to spot the bug. Being able to spot these things makes it much less likely that students will replicate these bugs in their own code during problem-solving.