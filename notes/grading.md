---
layout: left
---

# CS50 AP Workshop 2017

## The CS50 AP Classroom

### Introductions
- David Malan discusses how the grading session will be conducted.

### Grading Overview
- CS50 evaluates code based on the three axis.
  - Correctness
    - most objective
    - `check50` evaluates Correctness
      - Ran automatically by `submit50`
        - These grades can be overwritten for corner cases.
  - Design
    - most qualitative and subjective
    - With large groups of students, grading for Design can be a daunting task.
  - Style
    - Like Correctness, Style has its own tool for evaluation, `style50`.
      - Also ran automatically by `submit50` and rewritable.
    - Based on the [CS50 Style Guide](https://manual.cs50.net/style)

### Grading Tools
- GitHub
  - Traditionally used in industry for code reviews,
  - Allows for more qualitative feedback on code.
  - When students submit their code using `submit50`, their code becomes accessible on GitHub,
    - You can add comments to any line of code by clicking the red checkmark next to the line.
      - Students will be notified via email of any new comments.
      - This process can create dialog.

### Academic Honesty
- _This course’s philosophy on academic honesty is best stated as “be reasonable.”
- _... you may ask classmates and others for help so long as that help does not reduce to another doing your work for you._
  - Good rule of thumb.
- _Generally speaking, when asking for help, you may show your code to others, but you may not view theirs..._
  - Heuristic for whether something crosses the line.
  - "Let me see how you did it" is not okay.
- All academic honest problems reduce to making a poor split-second decision.
  - CS50 deals with this in a few ways.
    - regret clause
      - If you do cross the line and do something unreasonable, then come forward within 72 hours.
        - 72 is somewhat arbitrary, but enough time for students to sleep and think about what they've done.
        - This creates dialog and teachable moments.
        - The assignment is given a zero, but no further disciplinary action is pursued.
        - If need be, additional support is sought if there are issues outside of class causing stress
      - time consuming
  - 0-10% of CS50 students still cross the line.
    - This happens in cases where code was undoubtedly copied.
      - The red flags are usually repeated odd english errors or peculiar variable names that are shared.
      - Software helps catch similarities.
      - Ultimately, human judgement decides when the line has been crossed.

<img src="kitten.jpg" "kitten" width="200">

### Grading and Assessment
- Erin Carvalho takes over to talk more about grading practices in CS50.

#### Three Axes
- Correctness
  - Important that students have access to `check50` to check their work.
    - Students should get a perfect score in correctness with access to this tool.
- Design
  - Where most of the time will be spent grading.
    - most difficult
    - subjective
- Style
  - Both style and Correctness can be overwritten by the teacher.
    - In CS50x Nicaragua, students were failing hello.c checks as they were printing out "hola, mundo" (which, of course, is "hello, world" in Spanish).
      - This would be a good time to overwrite the Correctness grades.
  - If you wish to have another metric for grade style than the CS50 Style Guide, feel free to.
- Scope was removed because it became redundant with Correctness.
- Each recommended grading rubric has guidelines.
  - CS50 staff experience with common mistakes and design insight are built into these guidelines.
- Having students resubmit assignments to create a culture of error can be helpful.
  - Students are often more comfortable using functions and complex structures the second time around.
- The important take away from the three-axis model is that we don’t want to punish students for the same mistake over and over.
  - This is why the three axes are separate from each other.
  - Students shouldn't be punished for the same mistake several times.
- Grade each axis in as much of a vacuum as you can.
  - For example, when grading for Correctness, ignore Style and Design.

##### Five Point Scale
- CS50 uses a Five Point Scale to grade the Three Axes.

|                 Description                | Score |
|:------------------------------------------:|:-----:|
| Best. Essentially no room for improvement. |   5   |
|     Better. Minor room for improvement.    |   4   |
|      Good. Some room for improvement.      |   3   |
|      Fair. Ample room for improvement.     |   2   |
|                    Poor.                   |   1   |
|                 No attempt.                |   0   |

- 5s are rarely given, especially early on in the course.
  - There is always room for improvement.
- It's hard to instill in students that 3 is a good score.
  - Could only use Best, Better, etc. instead of numbers.

##### Correctness
- "To what extent is your code consistent with our specifications and free of bugs?"

<img src="correctness5.png" alt="correctness 5" width="600">
- 4 & 5 are the goal.
- 2 & 3 are where improvement can be made.
- 0 & 1 are for when students put minimal effort, just copy distribution code, or the program doesn't compile.
  - `check50` makes these grades harder to get.

##### `check50`
- Command-line tool built into CS50 IDE to run automated checks of students’ code.
- Currently undergoing a facelift.
- Students have access to `check50` for many of CS50’s problems, and are encouraged to use it to benchmark their programs.
- `check50` is used to grade correctness, but its output should be treated as suggestive, not determinative.

##### Design
- “To what extent is your code written well (i.e., clearly, efficiently, elegantly, and/or logically)?”

<img src="design5.png" alt="design5" width="600">
- 3 is a great place to be in terms of design.
- Hardest for students to understand, so its important to model what good design looks like.
- The most subjective of the three axes.
- Amorphous, evolving. What may have once been considered good design may now generally be considered poor.
- Of the three axes, this will likely be the most time-consuming to assess.
  - This is the type of feedback you want your students to get.
    - Why uses a while loop instead of a for loop? etc.
  - GitHub makes this process easier.
- Students will benefit most from qualitative feedback most here (e.g., comments/notes on cs50.me submissions page), so they can apply those comments in the future.
- Questions to consider (among others):
  - ~~Do I see repetition here that could be eliminated?~~
  - ~~Do I see loops here that could be eliminated?~~
  - ~~Are there magic numbers (hard-coded constants) that could be eliminated?~~
  - Can I eliminate:
    - repetition
    - loops
    - magic numbers
  - Is there a “shorter” way to accomplish the same thing?
    - Length of code is a good starting place for determining design.
  - Should this code have been broken out into its own function?
    - Students don't like to use functions immediately.
  - If you can answer yes to any of those questions, a perfect design score is probably not in the cards.

###### Design Example - Good
```c
while (change > 0) {   
    if (change >= 25) {      
        change -= 25;      
        coins++;
    }
    else if (change >= 10) {      
        change -= 10;      
        coins++;   
    }   
    else if (change >= 5) {      
        change -= 5;      
        coins++;   
    }   
    else {      
        change--;      
        coins++;   
    }
}
```
- One large loop, lots of branches to check on each iteration.
- `coins++` is “common code”. Could be factored out and moved to the end of the loop.
  - This is actionable feedback.

###### Design Example - Better
```c
while (change >= 25) {   
    change -= 25;   
    coins++;
}
while (change >= 10) {   
    change -= 10;   
    coins++;
}
if (change >= 5) {   
    change -= 5;   
    coins++;
}
coins += change;
```
- Uses magic numbers for quarters, dimes, and nickels.
- Loops have one small, simple task. No multi-fork branching.
- Recognizes you can only ever have one nickel. Clever shortcut.
- Recognizes that everything left behind after nickels must be pennies.

###### Design Example - Best? Part 1
```c
coins += (change / 25);
change %= 25;
coins += (change / 10);
change %= 10;
coins += (change / 5);
change %= 5;
coins += change;
```
- No loops at all; leverages C’s rules regarding integer division.
- Very short; code length is usually, but not always, a good proxy for design

###### Design Example - Best? Part 2
```c
#define QUARTER 25
#define DIME 10
#define NICKEL 5

coins += (change / QUARTER);
change %= QUARTER;
coins += (change / DIME);
change %= DIME;
coins += (change / NICKEL);
change %= NICKEL;
coins += change;
```

###### Design Example - Best? Part 3
```c
#define DENOMINATIONS 3
int values[] = {25, 10, 5};

for(int i = 0; i < DENOMINATIONS; i++)
{     
    coins += (change / values[i]);     
    change %= values[i];
}
```

##### Style
- "To what extent is your code readable (i.e., commented and intended with variables aptly named?”
- The next-most subjective of the three axes, though we have a recommended style guide.
- Students have access to `style50`, and are encouraged to use it to benchmark their programs for good style against our style guide.
- Used to grade style but, like `check50`, its output should be treated as suggestive but not determinative.
