# Chapter 4: Design, Elegance, and Efficiency
(Completion Time: 4 Weeks)

## Central Focus
Students will find patterns and test hypotheses based on given data, and then manipulate the data to extrapolate different results. In this process students will also identify multiple levels of abstraction with distribution as well as their own.

---

## a. Principles of Good Design
_Good design is what differentiates between a program that works and a program that works well. Good design is key aspect for a program to be portable, scalable, and reusable. Good design includes, but is not limited to, a program that has a fast run-time, is modularized for easy debugging, robust, consistent, and not repetitive in code._

### How to Launch the Lesson:
Break students up into groups and assign each group a different problem they have already done (i.e. Mario or Greedy). How can we leverage new concepts to make our programs more efficient? Did our previous solutions exhibit good design?

#### Activity: Switching Roles
Find some code examples or use anonymous student submissions from previous problems. Discuss what grade that submission would receive on the four axes of grading (correctness, scope, style and design). Focus particularly on design and what optimizations could make the program better.

##### Materials:
1. Code examples
2. Rubrics and/or descriptions for grading on each axis

---

## b. ncurses
_ncurses is a simple (albeit dated!) graphics library that can be used to create rudimentary graphical user interfaces (GUI) for games. Although rarely if at all used today, ncurses is among the most sophisticated graphics libraries we can use on CS50 IDE._

### How to Launch the Lesson:
Since students are already pretty familiar with the IDE at this point, spend some time going over some code examples using ncurses, including but not limited to:
      
* [hello.c](https://www.dropbox.com/s/0w6nbf86cioy1jq/hello.c?dl=0)
* [diagonals.c](https://www.dropbox.com/s/48ft084ye5p4eqs/diagonals.c?dl=0)
* [colors.c](https://www.dropbox.com/s/hrlxdm3kbsgbx2u/colors.c?dl=0)

---

## c. Structures and Encapsulation
_At a certain point, the usual suspect data types no longer suffice for the kind of work we need to do. Rather, we need to be able to encapsulate data more broadly, allowing us to group information together, but where all of that information relates to some large entity._

### How to Launch the Lesson:
Revisit arrays with students. What did they store? What were their limitations? Is there a way to group elements with the same indexes from separate arrays? What might that look like? Propose creating a new data type that can consist of multiple parts such a data type called "student" that consists of a "name", "ID #" and "birthdate."

---

## d. Recursion
_Recursive solutions to problems are typically contrasted with iterative solutions to problems. In a recursive solution, a function (or set of functions) repeatedly invokes slightly modified instance of itself, with each subsequent instance tending closer and closer to a base case._

### How to Launch the Lesson:
Break students up into groups and have them design a program using loops to find the factorial of a number, n (Example: 5! = 5*4*3*2*1). Then as a class describe how they can modify their solutions to use a recursive function instead of loops. For inspiration, watch:
      
* [sigma-0](https://www.youtube.com/watch?v=C-J0fKmwKmw)
* [sigma-1](https://www.youtube.com/watch?v=GSY5bEv3gX8)
      
#### Activity: Pass the Candy
Start with bags of varying numbers of small items (like candy or marbles), one for each student. In groups of 3-4, have each student record the number of items each person in the group has. Students should then give half of their items (determine whether students should round up or down for odd numbers) to the neighbor on their left and record new totals. Continue this for several iterations. How can we describe this process using a recursive approach? Watch this video to see how its done - https://www.youtube.com/watch?v=eiJ5-gUsNEQ.

##### Materials:
1. Bags of small items varying in number
2. Paper to record data

---

## e. Merge Sort
_The other sorting algorithms we've covered in the class -- selection sort, insertion sort, and bubble sort -- all suffer from the same general limitations and thus suffer the same, generally slow, worst-case runtime of O(n). Merge sort, though, behaves in a fundamentally different manner, leveraging recursion to "pass the buck" of sorting but also accomplishing something drastically superior -- O(n log n) runtime._

### How to Launch the Lesson:
As with all other sorting algorithms, having students participate in a live-action sort, such as by student height or by students simply holding numbered pieces of paper, is a good way to visualize this algorithm.

---

## f. Hexadecimal
_As previously discussed, analogies are made to the decimal (base 10) number system with which students are intimately familiar. You'll also learn how to represent values in hex and how to convert between hex, binary, and decimal using basic algorithms._

### How to Launch the Lesson:
Have students think back to binary. What are the place values in binary? How can we apply this to a hexadecimal system (base 16). What number(s) are represented the same in both systems. What would the place values be in hexadecimal?

#### Activity: Base Converter
Have students practice changing bases with this [interactive widget](http://bit.ly/2bE2cME). Click on game mode to randomly generate a number that students have to express in the base (2-binary, 16-hexadecimal, and 10-decimal) selected.

---

## g. File I/O
_Indeed, C has the capability of file I/O as a means of storing persistent data that exists after our programs have finished running and to read information from a file during the course of the program's execution. Students will be introduced to some of the basic file I/O functions they have at their disposal through stdio.h._

### How to Launch the Lesson:
Have students write the process of how they would normally write to a file. For instance: open a word doc, start typing, close word doc. Discuss implications of doing any of these processes out of order. Use this time to show some code examples of fopen, fread, fwrite and fclose. Some can be found [here](https://cdn.cs50.net/2014/fall/sections/4/section4.pdf).

---

## h. Images
_Images are stored as a number of file types, including but not limited to bitmaps (.bmp), JPGs (.jpg), PNGs (.png), and GIFs (.gif). Each type of file has its advantages and disadvantages, limitations, and more._

### How to Launch the Lesson:
Hand out grid paper to students. Have students create drawings that are made up of colored boxes (no partially colored boxes, either fully colored or empty). Explain that this is how computers view images (even high-quality ones). Each box represents a pixel that is either turned on or off.

#### Demo: Bit Examiner
Use the command line utility `xxd` on a small bitmap in the terminal to examine the bits.

#### Demo: Image Compressor
Compress a JPG multiple times (using regular Windows or OSX image tools) so students can see how it does not do well with compression when you try to "recover" the original.

##### Materials:
1. Sample images
2. Program to compress images

---

## i. Version Control
_Discuss different popular techniques for collaboration among programmers. The "driver/navigator" model will suffice for student collaboration, but we also touch on some more advanced techniques for those of you who wish to independently pursue their learning about these._

### How to Launch the Lesson:
Introduce students to the value of collaboration in coding with this [short video](https://www.youtube.com/watch?v=vgkahOzFH2Q).
