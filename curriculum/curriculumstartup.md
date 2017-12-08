# CS50 AP Curriculum Outline and Startup Guide

## Concepts Taught in CS50 AP

CS50 AP covers a lot of material. Luckily, we've got your back!

image:assets/igotu.gif[igotu,250]

The following is an outline of concepts covered in the CS50 AP curriculum. The individual conecpts are grouped into chapters with approximations for completion time. Each concept includes an tips and suggestions as to how to get started when teaching the topic.

### Chapter 0: Computers and Computing (Completion Time: 3 Weeks)

#### Central Focus
Students will engage in real world problems to analyze and create algorithms. Students will also explore the role of computers in today?s society and how they pertain to developments other fields.

---

#### a. Computers
_What makes a computer a computer? Discuss the common bonds that unify all those things, which we call computers. Also take a brief look at algorithms and the techniques used for solving problems._

.How to Launch the Lesson:
https://www.youtube.com/watch?v=Rs-Eub0-cRk, https://www.youtube.com/v/LHdVkPrdRYg, https://www.youtube.com/v/GcDshWmhF4A +
After watching the following videos, students can discuss in pairs or small groups what makes a device a computer. Start with a few math computations (addition, subtraction, multiplication, division, etc.) and have students try to come up with a formal definition of computation.

.Activity: Computer or Not?
Have students discuss and/or debate whether or not a device is a computer or not. This can be used as an opportunity for collaboration. Divide students into two groups and have them come up with a persuasive defense to present to the class.

Materials:

. Plethora of gadgets (some computers and some that are clearly not)
. Devices that straddle the line to initiate conversation on the definition of a computer (e.g., a set of chemical pool water testing strips, a smoke detector, an analog clock)

---

#### b. How Computers Work
_Take a look at the technical side about what's going on underneath the hood, so students are able to speak competently about it in conversations with others._

.How to Launch the Lesson:
Have students make predictions of what happens when a button is pressed or the mouse is clicked on their computers. Then using an old, obsolete computer, show students key components of computers and discuss their role with the system.

---

#### c. Bits and Bytes
_Data and storage on a computer all boils down to a fundamental unit of measure -- the bit, which can only take on two possible values. By combining bits into larger and larger groups we can become substantially more expressive._

.How to Launch the Lesson:
. Show students the development of memory storage. Some examples include floppy disks and zip disks which can be taken apart to show where things have been stored. More modern examples include CDs and external hard drives.

.Demo: Storage
Describe that a bit represents one of two values (e.g. true or false, on or off). Elaborate on the physical size various units of storage might take up, all things being equal. For example, if a single bit were about the size of a single marble filled with water:

* 1 bit -- a marble full of water
* 1 byte -- 1/8 cup water
* 1 kilobyte -- 9 gallons of water
* 1 megabyte -- an above ground swimming pool full of water
* 1 gigabyte -- a football field sized-pool of water, three feet deep
* 1 terabyte -- a football field sized-pool of water, half a mile deep

---

#### d. Hardware (Optional)
_Dive deeper into hardware and give students a consumer-oriented perspective on things to consider when we are purchasing or building their own machines._

.How to Launch the Lesson:
. Have students make a list of hardware that they have heard of, then using an old computer, disassemble and identify parts students have mentioned as well as parts they have not and discuss their purpose.

.Activity: Tech Shopping
Discuss the specs of tech items on the market. For further analysis, break students into groups and give them all a ?budget? to buy a computer. Challenge them to see who can get the most bang for their buck. Have them defend their choices and sacrifices made to the rest of the class.
Materials:
Devices for researching new technologies

---

#### e. Memory
_Understand the five major types of memory that are part of nearly every computer system are discussed -- hard disk drives (HDD), random-access memory (RAM), L2 and L1 cache, and the small bank of memory inside of a CPU._

.How to Launch the Lesson:
. Have students discuss memory specs of the devices that they use (i.e. iPhone, Android, MacBook Pro, etc.). Why are there two different numbers associated with memory? Have students predict what each might be and what information it stores.

---

#### f. Binary
_An introduction of binary numbers showing analogies to the decimal number system with the purpose to not only introduce students to binary numbers, but also prepare them for encountering other number systems._

.How to Launch the Lesson:
. Review decimal system and the concept of place values, then show students the place values for the binary system. Discuss what patterns students notice. Using 5 sheets of paper with the following values: 1, 2, 4, 8 and 16 flip some over and have students add the numbers to determine its decimal conversion. Then switch the game and give students decimal numbers to represent using the papers.

.Activity: Binary Bulbs
Light the way for students to understand binary with some physical representation. Have individual students represent different place values and give them numbers to represent by simply turning their light on or off.

Materials:

. Lights of sort (i.e. flashlights, light bulbs, lamps, etc.)

---

#### g. ASCII
_A look at how binary numbers can represent characters and punctuation as well as the standardization of such values in ASCII._

.How to Launch the Lesson:
. Review binary system from previous model. In small groups have students discuss how a computer might represent letters or symbols if can only understand 0s and 1s. Compare different groups responses. Would ?a? be represented in the same way in all systems? Show students ASCII table and discuss standardization and patterns.

.Activity: Crack the Code
In small groups have students write secret messages in ASCII (in decimal and/or binary) and have other groups try to crack them.

Materials:

. Paper and pen or whiteboards

---

#### h. Algorithms
_Learn to express algorithms using spoken or written language, and learn of the importance of defining algorithms precisely in order to have the desired effect(s) occur._

.How to Launch the Lesson:
Have students recreate a simple line image based on instructions given by a student. Only the student giving directions is aloud to see the original image. Display different student examples to stress the importance of using specific terminology.

.Demo: Phone Book
Show an example of linear search. Have students discuss with a partner or group what other algorithms could be both more efficient and correct. Discuss and demonstrate binary search while comparing it to linear search. Have students reflect on why the method of ripping the phone book is called binary search (e.g. what does binary search entail).

Materials:

. Phone book

.Activity: PB & J Sandwich Algorithm
Demonstrate the precision required for an algorithm to be carried out by a computer. Have one student record steps as a few student volunteers and a student teacher or principle execute the steps as literally as possible. Stop after 15-20 steps to discuss what went wrong and the importance of precision.

Materials:

. bag of bread
. peanut butter
. jam
. butter knife
. plate

.Activity: Creating Algorithms
Have students write an algorithm for completing some task they do every day. Have students submit their algorithms to you during class. If an interesting one comes up, ask two other students to volunteer. Have one follow the algorithm while the other is out of the room. Then have the second come in and execute the algorithm. Did the two executions play out identically?

.Activity: Everyday Algorgithms in Real Life
Have students use their written assignment 0-2. Students should volunteer to demonstrate another student?s algorithm, to illustrate how quickly things can go off track. If a student turns in a particularly compelling algorithm (an interesting task), it may be worth bringing in materials so that the instructions can be carried out.

---

### The AP CSP Explore Task
The Explore Task falls is a written assignment between Chapters 0 and 1. Students investigate a technology of their choosingAt this point they have completed several writing assignments geared towards helping students find credible sources and guiding them through the researching process.

---

### Chapter 1: Building Blocks of Programming (Completion Time: 4 Weeks)

#### Central Focus

Students begin to apply computational thinking, learning to express ideas first in pseudocode, then a visual language, Scratch, and finally, a text based language, C. They are introduced to various programming elements, and begin writing basic programs with proper syntax.

---

#### a. Pseudocode
_An introductions into express computational ideas in a language that can be translated to code. Used correctly, thinking in pseudocode may also help find bugs in your program before you even begin writing a single line of code!_

.How to Launch the Lesson:
Have students choose an algorithmic math procedure they know how to do (For example, solving the quadratic equation), and have them express the procedure in words. If there?s time, students can swap procedures and try to guess what the written procedure is supposed to do.

---

#### b. Scratch
_Create your first program using a drag and drop block based language called Scratch, which will allow students to learn concepts without getting mired in syntax._

.How to Launch the Lesson:
Because this topic is very specific, a teacher could introduce Scratch by having students play some games created in Scratch, either individually or as a class. The game used in lecture is: https://scratch.mit.edu/projects/76196420/

---

#### c. Syntax
_Moving away from a block-based language and more toward C, students will explore the details of how to express programming concepts in a text based language._

.How to Launch the Lesson:
Prepare syntactically incorrect English sentences (missing punctuation, etc). Have students try to decode their meaning. Are there sentences that could mean more than one thing? Explain why computers cannot compile programs with incorrect syntax.

.Demo: Error Checking
As David does in lecture, start with a simple but syntactically correct program. Then, add functionality to it but make syntax errors along the way, soliciting input from the class to fix them.

---

#### d. Variables
_Develop an understanding of a variable as a container in which you can store things. Students will then be able to use and update their variables throughout the program._

.How to Launch the Lesson:

Run a demonstration where selected students try to sum up a number via one sheet of paper without talking. Invite around 4 students to the front, and draw a box on the whiteboard. The first student writes a value there. The other students write a number value on a sheet of paper. Have each student add their number to the number on the board, thus updating the variable.

---

#### e. Data Types
_Every time students declare a variable they must bringing it into existence and specify its type. Students will explore the different variable types in C as well as the differences between static and dynamic typing._

.How to Launch the Lesson:
Have students think of a list of how many types of data they think a computer can store. Likely, you'll end up with responses like pictures or videos which is an opportunity to revisit how bits and bytes store data.

---

#### f. Operators
_Showing how we program arithmetic and assignment operations while noting the idiosyncrasies of left gets right where the expression x = 10 means x gets the value of 10._

.How to Launch the Lesson:
Have students think about operations from math. Have them review the order of operations. Use examples of expressions with similar numbers and operations but different parentheses to show the importance of placement both in math and computer science alike.

---

#### g. Boolean Expressions and Conditionals
_Conditional branching using Boolean expressions are how we as programmers make decisions in our programs. They empower us to take different forks in the road, allowing for different behaviors or different user experiences._

.How to Launch the Lesson:
Have students articulate how they have their scratch programs make decisions. When have we decided the cat should meow? (Using a Boolean).

---

#### h. Loops
_Instead of copying and pasting the same line(s) of code back-to-back, which can get clunky. All modern programming languages contain some variations on the construction of a loop, which permits iteration and repetition._

.How to Launch the Lesson:
Have students list the most repetitive tasks they have to do in everyday life (for instance, folding each t-shirt, washing each dish, etc). Discuss when would loops be useful in a real-world context.

.Activity: While Loops in Real Life
Have a student instruct another student to walk from one location to another location in the room. The challenge: You can only instruct one step at a time. Then, introduce loops and conditions, so that the statement "walk forward until you reach a wall" is valid.

---

### Chapter 2: Putting the Blocks Together (Completion Time: 5 Weeks)
#### Central Focus
Students dive deeper into abstraction and the efficiencies they provide. Students will become more familiar with the CS50 IDE and resources available to them within the IDE.

---

#### a. Compiling
_Look behind the curtain of make so students get a better understanding of the underlying compiler, clang, and the usefulness of having a program like make to abstract away creating that mashup of 0s and 1s, possibly linking together your code with the code of others._

.How to Launch the Lesson:
Explain the role of a compiler to students. Have them work in small groups to discuss metaphors for the role of a compiler. An example could be explaining that compilers are similar to translators. When two people who don?t communicate in the same language, they need a translator so that they can speak to one another. Students should be able to defend their own metaphors to other groups or the class at large.

.Demo: Compilation Simulation
Breaking down a simple program like Rob does in the short video is a good illustration of what happens at every step of the way with the compilation process.

---

#### b. Functions
_Introduce students to the simplification and elegance that functions provide us with. Discuss how to declare, define, and call functions and ways to modify them by way of parameters. (Note: This is a very important topic and might be worthwhile to spend about a week's time of class here.)_

.How to Launch the Lesson:
Have small groups of students come up with some sample inputs and outputs and have them switch amongst themselves. Can the other group(s) figure out the function based on the samples given? Explain how functions are often a black box of sorts. We don't need to always know how they work but we do need to know what it will output when given a specific input.

.Demo: Student Functions

Have students play the role of various functions, using pieces of paper as the "variables" they pass back and forth, to illustrate the notion of parameters, return values, and scope.

 Materials:
 1. Papers to write variables
 
.Activity: IDE Errors
Have students experiment with writing functions without declaring them and trying to compile their program, just to become familiar with some of the compiler errors that might get thrown.

Materials:

. Devices for using the IDE
. Feel free to use any of the source code on https://cs50.tv[cs50.tv] such as http://cdn.cs50.net/2014/fall/lectures/2/m/src2m/function-0.c[function 0] or http://cdn.cs50.net/2014/fall/lectures/2/m/src2m/function-1.c[function 1]

---

#### c. Arrays and Strings
_Arrays hold values of the same type at contiguous memory locations. In particular, the use of arrays allows us to create "groups" of variables without naming each, but still allowing us to individually index into the elements of the array. (Note: CS50 AP and C are 0 indexed, however College Board's AP Exam is 1 indexed)_

.How to Launch the Lesson:
Have students make predictions about how they would expect a computer to store data of the same type that is related. Would they want this data in multiple places or in one place? Would you want to have access to any piece at any given time or only one data point at a time while iterating through the each item? Have we already seen examples of this (i.e. strings)? Have students think-pair-share their responses.

.Activity: Multiplication Arrays
Use arrays to define a multiplication table, to give some exposure to multi-dimensional arrays. Have students the index for answer to a given multiplication answer such as 3*4 = table(4)(5) =12. (Note: arrays in C are 0 indexed)

.Activity: Game Mode
Have students draw out and play games they are already familiar with in the context of arrays. Some games include battleship, tic tac toe, and wheel of fortune. All of the games mentioned above can help students better visualize how data is stored in an array.

Materials:

. Paper and pen or whiteboards

---

#### d. Command-Line Interaction
_Look into ways we can collect input from the user before the program starts running, perhaps allowing the program to take different paths through the code depending on what the user provided at the command line._

.How to Launch the Lesson:
Is it better to get input from a user before the program runs or during? Break students up into two groups and have each defend a side. Might there be different scenarios where one might be more useful than the other.

.Demo: Mastering the Command Line
The good news here is that this topic tends to be among the least complicated, we've found, in CS50. Writing a few simple programs tends to go quite a long way. To that end, please feel free to use any of the below or others you find on https://cs50.tv[cs50.tv]:

. http://cdn.cs50.net/2014/fall/lectures/3/m/src3m/hello-3.c[hello 3]
. http://cdn.cs50.net/2014/fall/lectures/3/m/src3m/argv-0.c[argv 0]
. http://cdn.cs50.net/2014/fall/lectures/3/m/src3m/argv-1.c[argv 1]
. http://cdn.cs50.net/2014/fall/lectures/3/m/src3m/argv-2.c[argv 2]

---

#### e. Exit Codes
_Discuss the meanings of return 0; or return 1; and touch on why and how we might use them as programmers._

.How to Launch the Lesson:
Have students review return values from functions unit. In small groups have them discuss when one might want to exit a program. How would your program know how to exit? Would you want your program to always return the same value when it exits or would you want different values?

---

#### f. Libraries
_Show students the importance of using libraries and making use of the work that others before us have done and allowing us to spring forth from there._

.How to Launch the Lesson:
Ask students to create instructions to build something like a paper airplane or the like. Specify in their instructions that they are not allowed to use abstractions such as _triangle_, _square_, or _fold_. How tedious is this process to describe the same function repeatedly. Would it be easier if you were provided with some functions that the user already knew such as _fold_ or _right angle_.

.Activity: Exploring the IDE
Encourage students to poke around their IDE to have a look at the contents of the C standard library files, so they know what functions they have available to them. Knowledge is power! +

To do this, students must first cd /usr/include.

Then, they may type less <header file>, e.g. less stdio.h or less cs50.h, they can then scroll up and down in the terminal window to see the contents. So as to prevent accidental overwrites, the header files cannot be opened in Ace.

Type q to exit the less command and return to the terminal prompt. To return to their workspaces, students can type cd ~/workspace. It could also be useful for students to search the internet for other useful libraries that are not built into C or CS50 IDE, and identify the context in which one might wish to use functions from those libraries.

---

#### g. Typecasting
_C gives us the ability to cast (temporarily change) one data type into another with the same or less precision (e.g. we can cast a double to a float, but not vice versa), which might be more efficient from a design standpoint. Examine the mechanism and some use cases for typecasting._

.How to Launch the Lesson:
Review data types. Have students brainstorm as many scenarios as they can in which you would have a user input data in one type but want it in a different type later in the program.

---

#### h. Bugs and Debugging
_Explore different kinds of bugs, the real-world implications of buggy code, and techniques for rooting out bugs in our programs using certain tools built into CS50 IDE, in particular a popular command-line (and, in CS50 IDE, graphical) program called GDB._

.How to Launch the Lesson:
Pair students and have them share the strategies they have been using to debug their own programs. Switch students and have them share in different pairs. Are there similarities? Differences? Are there some methods that are more effective and more efficient than others?

.Demo: Exterminating Bugs
One of the best things to do here, honestly, is to find buggy code on the internet. There are tons and tons of websites hosting deliberately buggy C code for exercises involving "spot the bug," and it's a great way to fill a class period. Similarly many quiz questions available on quizbank.cs50.net contain deliberately buggy code and challenge students to spot the bug. Being able to spot these things makes it much less likely that students will replicate these bugs in their own code during problem-solving.

---

### Chapter 3: Thinking Computationally (Completion Time: 3 Weeks)

#### Central Focus

Students will analyze algorithms to compare correctness, run times, efficiencies and inefficiencies. Students will also explore computational problems and explain the difference between solvable and unsolvable problems.

---

#### a. Linear Search
_Linear search is the most basic algorithm for searching that students will encounter in the course. This topic should be quite short, just enough to familiarize students with the concept of linear search!_

.How to Launch the Lesson:
Refer back to the phone book demo
Have students try the following game with linear search. What limitations do you face? Does it matter what side you start on?
https://www.khanacademy.org/computing/computer-science/algorithms/intro-to-algorithms/a/a-guessing-game

.Activity: Where's the 50?
The "Where's the 50?" game that David plays in lecture is usually a riot, either because it goes spectacularly well or spectacularly poorly. Have students flip papers lined up in an array to find the number 50.

Materials:

. Papers to cover numbers written on a chalkboard/whiteboard

---

#### b. Bubble Sort
_Consider a basic approach to sorting that narrows the scope of our problem to focusing on ordering just two elements at a time, instead of an entire array at a time._

.How to Launch the Lesson:
Have a student sort a stack of papers (alphabetically or numerically) then have class describe the algorithm used to sort the array. Discuss why one might want a sorted array vs. an unsorted one. Are there benefits to such an array?

Have a group of students hold an integer. Sort the array using the various sorting algorithms. Write out pseudocode for the algorithms and try to formalize into C as a class or in small groups.

---

#### c. Selection Sort
_Another approach to sorting whereby one minimizes the number of swaps required (relative to bubble sort), but substantially increases the amount of comparing required in order to sort a single element._

.How to Launch the Lesson:
Have a group of students hold an integer. Sort the array using the various sorting algorithms. Write out pseudocode for the algorithms and try to formalize into C as a class or in small groups.

---

#### d. Insertion Sort
_The last of the sorting algorithms that doesn't require us to iterate across the array multiple times (as selection and bubble sort do), but this benefit, of course, comes with its own additional costs._

.How to Launch the Lesson:
Have a group of students hold an integer. Sort the array using the various sorting algorithms. Write out pseudocode for the algorithms and try to formalize into C as a class or in small groups.

---

#### e. Binary Search
_Students discover an algorithm whose speed can be leaps and bounds better than linear search, but not without a cost--the data must be sorted first._

.How to Launch the Lesson:
Go back to the same page (https://www.khanacademy.org/computing/computer-science/algorithms/intro-to-algorithms/a/a-guessing-game) and look at the example containing 300 numbers. How is it possible to guess the computers answer in 9 guesses? How might we modify our algorithm leveraging Unit 0 concepts?

.Activity: Ping Pong Search
Also fairly dramatic is to do binary search with numbered ping-pong balls sitting on plastic cups, smacking away various portions of the "array" as you go through the search.

Materials:

. Ping pong balls
. Plastic cups

---

#### f. Time Complexity
_Begin to discuss the way in which computer scientists measure the theoretical worst-case (O) and best-case (W) scenarios when running programs._

.How to Launch the Lesson:
Compare bubble sort, insertion sort and selection sort for different arrays at https://www.toptal.com/developers/sorting-algorithms (number of data points and types of data are customizable). Which is fastest? Do they vary based on how sorted the data is? How do we assign meaning to these times? Given a large set of data which one would sort the fastest (trick question since they all have big O(n^2^))?

---

#### g. Unsolvable Problems
_Computers are amazing, and it seems like there must be nothing a computer cannot do. But as it turns out, computers can't do everything, and never actually will be able to. Spend some time considering some unsolvable problems in computer science, including one of the most famous problems in that category: the halting problem._

.How to Launch the Lesson:
Have students discuss a problem that computers cannot solve in pairs or small groups. Challenge students to think of a way that a computer could in fact solve that problem. Show students https://www.youtube.com/watch?v=92WHN-pAFCs and https://www.youtube.com/watch?v=macM_MtS_w4 to discuss problems in the realm of CS that are in fact unsolvable.

---

#### h. Simulation
_Computer programs can be used to create models and simulations, to test hypotheses and generate new understanding and knowledge. Students will explore simulations of existing knowledge and use simulation software to test models._

.How to Launch the Lesson:
In small groups, have students discuss what scenarios one might use a simulation to solve or simplify a problem. What benefits are afforded to us when we use simulations?

---

### Chapter 4: Design, Elegance, and Efficiency (Completion Time: 4 Weeks)
#### Central Focus

Students will find patterns and test hypotheses based on given data, and then manipulate the data to extrapolate different results. In this process students will also identify multiple levels of abstraction with distribution as well as their own.

---

#### a. Principles of Good Design
_Good design is what differentiates between a program that works and a program that works well. Good design is key aspect for a program to be portable, scalable, and reusable. Good design includes, but is not limited to, a program that has a fast run-time, is modularized for easy debugging, robust, consistent, and not repetitive in code._

.How to Launch the Lesson:
Break students up into groups and assign each group a different problem they have already done (i.e. Mario or Greedy). How can we leverage new concepts to make our programs more efficient? Did our previous solutions exhibit good design?

.Activity: Switching Roles
Find some code examples or use anonymous student submissions from previous problems. Discuss what grade that submission would receive on the four axes of grading (correctness, scope, style and design). Focus particularly on design and what optimizations could make the program better.

Materials:

. Code examples
. Rubrics and/or descriptions for grading on each axis

---

#### b. ncurses
_ncurses is a simple (albeit dated!) graphics library that can be used to create rudimentary graphical user interfaces (GUI) for games. Although rarely if at all used today, ncurses is among the most sophisticated graphics libraries we can use on CS50 IDE._

.How to Launch the Lesson:
Since students are already pretty familiar with the IDE at this point, spend some time going over some code examples using ncurses, including but not limited to:
      
      * https://www.dropbox.com/s/0w6nbf86cioy1jq/hello.c?dl=0[hello.c]
      * https://www.dropbox.com/s/48ft084ye5p4eqs/diagonals.c?dl=0[diagonals.c]
      * https://www.dropbox.com/s/hrlxdm3kbsgbx2u/colors.c?dl=0[colors.c]

---

#### c. Structures and Encapsulation
_At a certain point, the usual suspect data types no longer suffice for the kind of work we need to do. Rather, we need to be able to encapsulate data more broadly, allowing us to group information together, but where all of that information relates to some large entity._

.How to Launch the Lesson:
Revisit arrays with students. What did they store? What were their limitations? Is there a way to group elements with the same indexes from separate arrays? What might that look like? Propose creating a new data type that can consist of multiple parts such a data type called "student" that consists of a "name", "ID #" and "birthdate."

---

#### d. Recursion
_Recursive solutions to problems are typically contrasted with iterative solutions to problems. In a recursive solution, a function (or set of functions) repeatedly invokes slightly modified instance of itself, with each subsequent instance tending closer and closer to a base case._

.How to Launch the Lesson:
Break students up into groups and have them design a program using loops to find the factorial of a number, n (Example: 5! = 5*4*3*2*1). Then as a class describe how they can modify their solutions to use a recursive function instead of loops. For inspiration, watch:
      
      * https://www.youtube.com/watch?v=C-J0fKmwKmw[sigma-0]
      * https://www.youtube.com/watch?v=GSY5bEv3gX8[sigma-1]
      
.Activity: Pass the Candy
Start with bags of varying numbers of small items (like candy or marbles), one for each student. In groups of 3-4, have each student record the number of items each person in the group has. Students should then give half of their items (determine whether students should round up or down for odd numbers) to the neighbor on their left and record new totals. Continue this for several iterations. How can we describe this process using a recursive approach? Watch this video to see how its done - https://www.youtube.com/watch?v=eiJ5-gUsNEQ.

Materials:

. Bags of small items varying in number
. Paper to record data

---

#### e. Merge Sort
_The other sorting algorithms we've covered in the class -- selection sort, insertion sort, and bubble sort -- all suffer from the same general limitations and thus suffer the same, generally slow, worst-case runtime of O(n). Merge sort, though, behaves in a fundamentally different manner, leveraging recursion to "pass the buck" of sorting but also accomplishing something drastically superior -- O(n log n) runtime._

.How to Launch the Lesson:
As with all other sorting algorithms, having students participate in a live-action sort, such as by student height or by students simply holding numbered pieces of paper, is a good way to visualize this algorithm.

---

#### f. Hexadecimal
_As previously discussed, analogies are made to the decimal (base 10) number system with which students are intimately familiar. You'll also learn how to represent values in hex and how to convert between hex, binary, and decimal using basic algorithms._

.How to Launch the Lesson:
Have students think back to binary. What are the place values in binary? How can we apply this to a hexadecimal system (base 16). What number(s) are represented the same in both systems. What would the place values be in hexadecimal?

.Activity: Base Converter
Have students practice changing bases with this http://bit.ly/2bE2cME[interactive widget]. Click on game mode to randomly generate a number that students have to express in the base (2-binary, 16-hexadecimal, and 10-decimal) selected.

---

#### g. File I/O
_Indeed, C has the capability of file I/O as a means of storing persistent data that exists after our programs have finished running and to read information from a file during the course of the program's execution. Students will be introduced to some of the basic file I/O functions they have at their disposal through stdio.h._

.How to Launch the Lesson:
Have students write the process of how they would normally write to a file. For instance: open a word doc, start typing, close word doc. Discuss implications of doing any of these processes out of order. Use this time to show some code examples of fopen, fread, fwrite and fclose. Some can be found here -https://cdn.cs50.net/2014/fall/sections/4/section4.pdf.

---

#### h. Images
_Images are stored as a number of file types, including but not limited to bitmaps (.bmp), JPGs (.jpg), PNGs (.png), and GIFs (.gif). Each type of file has its advantages and disadvantages, limitations, and more._

.How to Launch the Lesson:
Hand out grid paper to students. Have students create drawings that are made up of colored boxes (no partially colored boxes, either fully colored or empty). Explain that this is how computers view images (even high-quality ones). Each box represents a pixel that is either turned on or off.

.Demo: Bit Examiner
Use the command line utility `xxd` on a small bitmap in the terminal to examine the bits.

.Demo: Image Compressor
Compress a JPG multiple times (using regular Windows or OSX image tools) so students can see how it does not do well with compression when you try to "recover" the original.

Materials:
. Sample images
. Program to compress images

---

#### i. Version Control
_Discuss different popular techniques for collaboration among programmers. The "driver/navigator" model will suffice for student collaboration, but we also touch on some more advanced techniques for those of you who wish to independently pursue their learning about these._

.How to Launch the Lesson:
Introduce students to the value of collaboration in coding with this https://www.youtube.com/watch?v=vgkahOzFH2Q[short video].

---

### Chapter A: Managing Data (Optional Track)
#### Central Focus
#### a. Stacks
#### b. Queues
#### c. Pointers
#### d. Dynamic Memory
#### e. Valgrind
#### f. Trees
#### g. Tries
#### h. Linked Lists
#### i. Hash Tables

### Chapter B: Developer’s Toolbox (Optional Track)
#### Central Focus
#### a. Abstraction and API
#### b. Data Compression
#### c. Huffman Coding
#### d. Scalability
#### e. Collaboration

### Chapter 5: Networking and the Internet (Completion Time: 3 Weeks)
#### Central Focus
Students will transition from programs that exist only on their IDE to programs that can be viewed globally. They will explore the global system of interconnected computer networks that use the Internet protocol suite (TCP/IP) to link devices worldwide and the languages which enable them to express their ideas on the internet.

---

#### a. Internet Basics
_An overview of how the internet works and how we as users interact with it. This topic can also be used as sort of a teaser for the rest of the chapter._

.How to Launch the Lesson:
Have students write down their ideas of how they think the internet works. Revisit these ideas at the end of this chapter. What was correct? What was incorrect? What do students still have questions about?

---

#### b. IP Addresses
_IP (Internet Protocol) addresses are assigned to each device connected to a network. A device or web page can be identified by its IP addresses, as all are unique - like a postal address._

.How to Launch the Lesson:
Have students find their IP addresses. Why does everyone on the internet need a unique IP address? Students can switch IP addresses with peers and try to track the location using http://what-is-my-address-ip.com/ or a similar site.

.Activity: Your IP Address
Have students find their IP addresses on their computer and connect to one another's addresses using the terminal command ping or something similar.

.Activity: Your Favorite IP Address
Have students find the IP addresses of their favorite websites and get to them by typing the IP address instead of the URL.

---

#### c. DNS and DHCP
_DHCP, also known as the Dynamic Host Configuration Protocol, dynamically assigns IP addresses to devices connecting to a network. DNS, the Domain Name System, is responsible for translating URLs of websites to IP addresses and vice versa. We need both IP addresses to be able to form a successful connection from sender to receiver._

.How to Launch the Lesson:
Have students think of metaphors that represent the roles that DHCP and DNS play with regards to IP addresses. Would it still be able to access websites without DHCP? or DNS? Are both necessary?

.Demo: Phone Book
An analogy for DNS to use is a phone book - you look up a person's name, and are given their phone number if you need to contact them. This is similar to typing in a website URL, which is then translated to an IP address.

.Demo: Dynamically Assigning Numbers
An analogy for DHCP could be anything dealing with dynamically assigning numbers to devices, i.e. numbers at a deli, characters in a board game, etc. The key is that it is possible to have the same number more than once, but that it is not guaranteed.

---

#### d. Routers
_Routers are the components of the Internet that direct packages of data across various networks. They follow a set of rules to direct packets based upon IP address and port. Typically routers will direct individual packets on different routes to end up at the same location._

.How to Launch the Lesson:
Let each student pick a unique website. Then use a site similar to http://www.yougetsignal.com/tools/visual-tracert/ to view the trace route for each site or do it from the command line. Which student had the furthest location in their trace route? Why do you think that is?

---

#### e. TCP and IP
_IP is the system we've just seen, that works with routers to ensure packets of data are split into pieces, sent to the correct destination, and pieced back together. TCP ensures data is properly marked when it is split into pieces, so if one packet does not arrive, the sender is notified and can resend._

.How to Launch the Lesson:
Using the same tool as above have students use the same web tool to count how many locations they went to in their trace route. Did number of places correspond with distance from the previous time using this tool? Why or why not would this make sense? Which website had the least number of hops? Which had the most?

.Activity: Connections
Give students all a notecard on which is written a different component of an internet connection. Some of them will be packets of data; see if the packets can get to their destination by having students place themselves in the correct order.

---

#### f. HTTP
_Hypertext Transfer Protocol, or HTTP, is what web browsers use to speak to web servers. The server receives the request and either successfully executes the action (by rendering a page or submitting a form, for example) or returns an error code; these are called HTTP status codes._

.How to Launch the Lesson:
Find examples of different types of requests. Load the pages with Developer Tools and display the requests to the students.

.Demo: Status Codes
Find examples of the different status codes on the web (most commonly a 404 or 403), and show them to your students using Chrome's Developer Tools or the like.

---

#### g. Trust Models and Open Source
_Every open source piece of software is held to an "open standard" that the software will work in the way intended and not do anything malicious. This involves a significant amount of trust on our end, that whenever we compile a program or visit a website, the pieces of software we use are not injecting malicious code into our computers._

.How to Launch the Lesson:
In small groups, have students research a downloadable software or song. Let them read through the terms and conditions. What sort of things do we agree to that one would be surprised to see? Are we more trusting of certain things than others? What is this trust based on?

---

#### h. Cybersecurity
_The Internet is a wonderful resource, but can also occasionally make us vulnerable if we are not following good practices. While we can limit vulnerability to attacks there are many security threats we cannot control and may not even be aware of._

.How to Launch the Lesson:
Students tend to identify with stories they've heard; try to find a cyberattack that has been in the news recently and talk about it! You can probably find a video and show that as well

.Demo: Insecurity
Find an insecure website (non-https) desiring input of a password or credit card number to show your students how easy it is to spoof something that looks secure.

.Demo: Permission Levels
If you can display webpages on your localhost to students, you can demonstrate different permission levels on a simple page, talking about why it is beneficial to keep some pages private and only the necessary ones public.

---

#### i. HTML
_HTML, or HyperText Markup Language, forms the backbone of web pages. It is used to make any web page you see by formatting all text and images. Students will learn how to create basic web pages using the language._

.How to Launch the Lesson:
Discuss the differences between a mark up language and programming languages. Why do we need two separate languages to do different things? Maybe have students play around with https://www.khanacademy.org/computing/computer-programming/html-css/intro-to-html/p/html-basics[Khan Academy's HTML module].

.Demo: Developer Tools
Take a look at an existing website using Chrome's Developer Tools and have your students figure out what the individual tags do.

---

#### j. CSS
_CSS, or Cascading Style Sheets, is used to style web pages. It is capable of manipulating colors, positioning, size, alignment, fonts, borders, background shading, and others._

.How to Launch the Lesson:
Have students discuss things that they were unable to do in HTML. Which of those things fall into a styling vs. programming language. How can CSS help? Maybe integrating aspects of https://www.khanacademy.org/computing/computer-programming/html-css/intro-to-css/p/css-basics[Khan Academy's module on CSS].

.Demo: Webpage 2.0
Similar to the HTML demonstration, you can create a simple webpage, this time including a CSS sheet to stylize.   

.Activity: Creativity
Create a simple activity that allows students to be creative with their styling; they can make a basic webpage and choose colors, fonts, shading, etc. 

---

### Chapter 6: Problem Solving in an Interconnected World (Completion Time: 5 Weeks)
#### Central Focus

Students will explore different aspects of building multilayered web pages such as those that manage data and have a back end. They will apply their knowledge of C to implement logic in new languages such as PHP, JavaScript, and Ajax.

#### a. Python
TODO

.How to Launch the Lesson:
TODO

.Demo: Python Spell-Checker
Implementing a spell-checker in PHP live in class can be a shocking and impactful demonstration, for those students who are familiar with the complexity of C's implementation. http://cdn.cs50.net/2015/fall/lectures/7/w/src7w/mispellings/

---

#### b. Python for Web Programming
TODO

.How to Launch the Lesson:
TODO

---

#### c. SQL
_SQL (the Structured Query Language) is a language that we can use to create, add to, select, modify, and delete information in connection with a database. By learning how to use SQL we can create a so-called "backend" for our websites, allowing us to store persistent user data (sort of like the notion of a FILE* in C) that we can access when necessary to improve the user experience on a page._

.How to Launch the Lesson:
Open up phpMyAdmin in your IDE and demonstrate each of the basic operations (SELECT, INSERT, UPDATE, DELETE) using the graphical tabs. Then repeat all of the basic operations only using the SQL tab to show the text based power, so students will be able to contemplate how they might access their databases programmatically.

---

#### d. MVC
_MVC, or the Model-View-Controller paradigm, is a software design practice that separates code for a website into three parts: the model code, the view code, and the controller code. The model code deals with the data of the website, often performing operations that interact with a database. The controller code is the logic of the website: it contains code like loops and conditions. The view code is the aesthetic part of the website: it takes information provided by the controller and displays the page that the user ultimately sees when they visit the website._

.How to Launch the Lesson:
Using an example website, have students in small groups break down the features of the site into three parts: model code, view code, controller code. The model code deals with the data of the website, often performing operations that interact with a database. The controller code is the logic of the website: it contains code like loops and conditions. The view code is the aesthetic part of the website: it takes information provided by the controller and displays the page that the user ultimately sees when they visit the website.

.Demo: Website 3
Make a simple website using the MVC paradigm, or have your students do it themselves for practice.

---

#### e. JavaScript
_Python gave us the opportunity to build dynamic websites, but JavaScript lets us take things even further, permitting client-side modifications to our web pages, making them more dynamic without requiring contact with a database or off-site server, which can greatly improve the user experience. In this module, students will get a very quick introduction to the basic power of JavaScript and the Document Object Model (DOM), which JavaScript is able to manipulate to literally change the contents of a website, albeit temporarily, in response to user interactions._

.How to Launch the Lesson:
Show students side by side of C, Python, and JavaScript. Once again discuss similarities and differences. Maybe even using the inspect element in Chrome and changing some of the JavaScript, HTML, and CSS to see live changes.

---

#### f. Ajax
_Ajax (which formerly stood for Asynchronous JavaScript and XML) is a web programming technique that lets us dynamically update the content of the web page. We can make snappier web pages that do not reload every time additional content is requested. Here, we see how this technique can be accomplished using Javascript, in which an HTTP request is made asynchronously (in the background) to the server, and a callback function handles the JSON (JavaScript Object Notation) object that is returned._

.How to Launch the Lesson:
Take the time to explain Client side and Server side systems. Have students find some examples of both. What are benefits and disadvantages of both?

---

#### g. Artificial Intelligence
_Artificial intelligence is an example of how Computer Science concepts can be used to create global impact. CS50's artificial intelligence material covers natural language processing, speech recognition, and game playing systems._

.How to Launch the Lesson:
Have students discuss preconceived notions of AIs in small groups. What is the difference between a clever algorithm and artificial intelligence? Discuss as a class which of these notions are correct and incorrect and explore why.

.Activity: Eliza
Have students attempt to converse with Eliza: 

* http://cdn.cs50.net/2015/fall/lectures/10/w/src10w/eliza.c.src[By compiling and running CS50's C code]. 
* http://nlp-addiction.com/eliza/[By using a web implementation]. 
* http://chayden.net/eliza/Eliza.html[By running a Java executable].

.Activity: A Problem with Machine Learning
Try to get your hands on a cheap device to turn your phone or mobile device into a means to watch VR video (such as google cardboard). You can even watch CS50 lectures in VR at video.cs50.net by changing the view mode in the bottom left corner. What fields might benefit from technologies like this?

---

#### h. Virtual and Augmented Reality
_Virtual and augmented reality has recently taken the world by storm. Virtual reality allows a user to jump into a three dimensional world so to speak to experience games, videos and other simulations in a new way. This year CS50 has produced all lectures in VR. If you go to https://video.cs50.net/ and click on the icon that looks like a VR headset you will experience lecture as though you are in Sander's theatre. Augmented reality is similar in spirit to virtual reality, only that instead of taking you away from your surroundings completely, the effects, videos, or games are over layed to tie in your surroundings with the technology. In this module, students will explore the difference between the two and discover what advances can be made with this technology._

.How to Launch the Lesson:
Try to get your hands on a cheap device to turn your phone or mobile device into a means to watch VR video (such as google cardboard). You can even watch CS50 lectures in VR at video.cs50.net by changing the view mode in the bottom left corner. What fields might benefit from technologies like this?

---

### The AP CSP Create Task

The Create Task comes in at the end of the core chapters, following Chapter 6. After completing Chapter 6, students have developed an entire toolbox of languages and platforms to build whatever they choose. While the majority of problems are very much structured and a have a well-defined solution, students engage a sense of creativity in the way that they implement their algorithms. Students understand that everyone may have a different approach to solving the same problem, but they could all be correct approaches. By the end of the course, students have dabbled in C and web development and have implemented algorithms to solve various problems. It is at this point that students are able to create a project that they are engaged in and are able to research new topics of interest that were not covered in-depth in the course.