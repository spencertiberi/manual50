# Chapter 3: Thinking Computationally
(Completion Time: 3 Weeks)

## Central Focus
Students will analyze algorithms to compare correctness, run times, efficiencies and inefficiencies. Students will also explore computational problems and explain the difference between solvable and unsolvable problems.

---

## a. Linear Search
_Linear search is the most basic algorithm for searching that students will encounter in the course. This topic should be quite short, just enough to familiarize students with the concept of linear search!_

### How to Launch the Lesson:
Refer back to the phone book demo
Have students try the following game with linear search. What limitations do you face? Does it matter what side you start on?
https://www.khanacademy.org/computing/computer-science/algorithms/intro-to-algorithms/a/a-guessing-game

#### Activity: Where's the 50?
The "Where's the 50?" game that David plays in lecture is usually a riot, either because it goes spectacularly well or spectacularly poorly. Have students flip papers lined up in an array to find the number 50.

##### Materials:
Papers to cover numbers written on a chalkboard/whiteboard

---

## b. Bubble Sort
_Consider a basic approach to sorting that narrows the scope of our problem to focusing on ordering just two elements at a time, instead of an entire array at a time._

### How to Launch the Lesson:
Have a student sort a stack of papers (alphabetically or numerically) then have class describe the algorithm used to sort the array. Discuss why one might want a sorted array vs. an unsorted one. Are there benefits to such an array?

Have a group of students hold an integer. Sort the array using the various sorting algorithms. Write out pseudocode for the algorithms and try to formalize into C as a class or in small groups.

---

## c. Selection Sort
_Another approach to sorting whereby one minimizes the number of swaps required (relative to bubble sort), but substantially increases the amount of comparing required in order to sort a single element._

### How to Launch the Lesson:
Have a group of students hold an integer. Sort the array using the various sorting algorithms. Write out pseudocode for the algorithms and try to formalize into C as a class or in small groups.

---

## d. Insertion Sort
_The last of the sorting algorithms that doesn't require us to iterate across the array multiple times (as selection and bubble sort do), but this benefit, of course, comes with its own additional costs._

### How to Launch the Lesson:
Have a group of students hold an integer. Sort the array using the various sorting algorithms. Write out pseudocode for the algorithms and try to formalize into C as a class or in small groups.

---

## e. Binary Search
_Students discover an algorithm whose speed can be leaps and bounds better than linear search, but not without a cost--the data must be sorted first._

### How to Launch the Lesson:
Go back to the same page (https://www.khanacademy.org/computing/computer-science/algorithms/intro-to-algorithms/a/a-guessing-game) and look at the example containing 300 numbers. How is it possible to guess the computers answer in 9 guesses? How might we modify our algorithm leveraging Unit 0 concepts?

#### Activity: Ping Pong Search
Also fairly dramatic is to do binary search with numbered ping-pong balls sitting on plastic cups, smacking away various portions of the "array" as you go through the search.

##### Materials:
1. Ping pong balls
2. Plastic cups

---

## f. Time Complexity
_Begin to discuss the way in which computer scientists measure the theoretical worst-case (O) and best-case (W) scenarios when running programs._

### How to Launch the Lesson:
Compare bubble sort, insertion sort and selection sort for different arrays at https://www.toptal.com/developers/sorting-algorithms (number of data points and types of data are customizable). Which is fastest? Do they vary based on how sorted the data is? How do we assign meaning to these times? Given a large set of data which one would sort the fastest (trick question since they all have big O(n<sup>2</sup>))?

---

## g. Unsolvable Problems
_Computers are amazing, and it seems like there must be nothing a computer cannot do. But as it turns out, computers can't do everything, and never actually will be able to. Spend some time considering some unsolvable problems in computer science, including one of the most famous problems in that category: the halting problem._

### How to Launch the Lesson:
Have students discuss a problem that computers cannot solve in pairs or small groups. Challenge students to think of a way that a computer could in fact solve that problem. Show students https://www.youtube.com/watch?v=92WHN-pAFCs and https://www.youtube.com/watch?v=macM_MtS_w4 to discuss problems in the realm of CS that are in fact unsolvable.

---

## h. Simulation
_Computer programs can be used to create models and simulations, to test hypotheses and generate new understanding and knowledge. Students will explore simulations of existing knowledge and use simulation software to test models._

### How to Launch the Lesson:
In small groups, have students discuss what scenarios one might use a simulation to solve or simplify a problem. What benefits are afforded to us when we use simulations?