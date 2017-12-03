---
layout: nav
---

# CS50 Grading

## Grading Axes
Just like on campus at Harvard, CS50 AP is graded along the following three axes:

* **Correctness:** the extent to which code is consistent with CS50 specifications and free of bugs.
* **Design:** the extent to which code is written well (i.e., clearly, efficiently, elegantly, and/or logically)
* **Style:** the extent to which code is readable (i.e., commented and intended with variables aptly named)

Out of the three, **Design** is the most subjective. Whereas **Correctness** and **Style** will be automatically handled by CS50.me and the related submission command, `submit50`, **Design** is graded solely by the teacher. Note that teachers can override the grades automatically assigned for **Correctness** and **Style**. In general, all 3 axes are graded using the course's five point scale.

### Five Point Grading Scale

When grading for the 3 axes, CS50 uses a five point grading scale for determining marks as follows:

| Level | Description                                |
|-------|--------------------------------------------|
| **5** | Best: Essentially no room for improvement. |
| **4** | Better: Minor room for improvement.        |
| **3** | Good: Some room for improvement.           |
| **2** | Fair: Ample room for improvement.          |
| **1** | Poor                                       |
| **0** | No Effort                                  |

<br>
NOTE: A grade of 3 is indeed good! This can take quite some time for students to get comfortable with as they have been trained to see 3 out of 5 as a percentage, namely 3/5 or 60%. +

Also, whereas scores of 5 can be common for **Correctness** and **Style**, a score of 5 for **Design** should be rare; a 5 here implies perfection. **Design**, by its nature, offers room for improvement in most cases.  Thus, a 4 for **Design** is a really good grade.  

In addition to leveraging this grading scheme, it's important to focus on providing quality feedback during the grading process so that grades have pedagogical value. Feedback should create opportunities for dialog between teachers and students.


## Giving Feedback
Grading for **Design** is by far the most time-consuming, albeit satisfying, process in grading for CS50 AP. The focus of grading for **Design** is the efficiency and elegance of a student's code. As such, feedback is important when grading **Design**. Of course, this feedback can also shine light on **Style** and **Correctness**.

Feedback should focus on pointing out good design practices (+s) and things to change (Δs). As a goal, there should be an 1-to-1 ratio of +s to Δs. It's essential that this feedback include reasoning as to why something is a good practice or should be changed.

In general, there should be an inverse relationship between feedback and score. That is, the lower the score, the more feedback should be provided, and visa versa.

### Feedback Examples
Note the following code segments from a submission by a fictitious student for the problem Greedy:

#### Design Feedback Opportunity
```c
 6    // all of the floats used in the program
 7    float quarter = 25;
 8    float dime = 10;
 9    float nickel = 5;
10    float penny = 1;
11    float owed = 0;
12    float coins = 0;
```
<img src="muppet.png" alt="CS50 Muppet" width="150" align="right">

> It's a great idea to store these reused values. Do these values ever change or are they static? Do they need to be floats?
> Perhaps it would be best to create constants using `#DEFINE`.
>
> -- Awesome CS50 AP Teacher

#### Another Design Feedback Opportunity

```c
25    while (owed >= quarter)
26    {
27        owed = owed - quarter;
28        coins++;
29    }
30    
31    while (owed >= dime && owed < quarter)
32    {
33        owed = owed - dime;
34        coins++;
35    }    
36    while (owed >= nickel && owed < dime)
37    {
38        owed = owed - nickel;
39        coins++;
40    }         
41    while (owed >= penny && owed < nickel)
42    {    
43        owed = owed - penny;
44        coins++;
45    }
```

<img src="dancoffey.gif" alt="Dan" width="150" align="right">

> How might we have used the modulus `%` operator instead of using while loops? What might be better about this approach?
>
> -- Handsome CS50 AP Teacher

#### Style Feedback Opportunity
```c
14    // asks for a input for the program
15    do
16    {
17    printf("How much change is due: ");
18    owed = GetFloat();
19    }
20    
21    // computer takes users change and converts into as few coins as possible    
22    while (owed <= 0);
```
<img src="mario.jpg" alt="Mario" width="150" align="right">

> Nice use of braces. However, on lines 17 and 18, it would be easier to read if the lines had another four spaces of indentation. Also,
> the comment on line 21 breaks
> up the do-while loop, making it harder to read. Best to describe this process with the comment on line 14.
>
> -- Fabulous CS50 AP Teacher

## Assigning a Score

It can take some practice to determine how to assign a five point scale grade for **Design**.  Thus, for each CS50 AP problem, grading guidelines are provided on the [CS50 AP Portal](https://ap.cs50.net/resources/).
