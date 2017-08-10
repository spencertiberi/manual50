---
layout: left
---

# CS50 AP Workshop 2017

## Checking for Understanding

### Introduction
- Doug Lloyd highlights the importance of checking for understanding, particularly for teachers who adopt CS50 materials for a flipped classroom environment.
- For a later session demonstrating a CS50 section, Doug asks the audience, by a show of hands, whether they would rather learn early material or web-based material.

### What is Checking for Understanding?
- Transitioning from the idea of "I taught it" to "they learned it."
  - The latter is harder and more important.
  - CS50 at Harvard has Less Comfortable and More Comfortable sections that students can self-select themselves into.
    - This helps differentiate pace effectively.
  - In a high school classroom, not everyone is coming in with the same level of preparedness.
    - No pretest is given for CS50.

### Challenges
- Compounding: material build on itself more than in many other subjects
  - Material in a CS class is extremely varied.
- Theoretical and practical knowledge: knowing the concept ≠ knowing how to write code for it.
  - For example, the concept of creating a hash table may be investigated in a short, but the code implementation is still up to the student.
  - Goal of CS50 teachers is to not give away too much of the practical implementation.
- Many ways to solve problems: many different "correct" solutions to problems.
  - Some are better designed than others.
  - Doug notes that every year he sees novel solutions to problem sets.
    - There is no right answer to the problem.
  - Important to make sure that a student's different thinking and implementation aren't hampered by teacher thinking.

### Strategies
- Frequent questioning
  - Uncomfortable silences
  - Socratic-style
    - Having conversation back and forth between the teacher and student.
- Practice problems
  - They are not the basics of actual assignments, but steps in the right direction.
- Resources to help reinforce concepts or refresh memory
  - CS50 recourses are available in a lot of different flavors:
    - Video, audio, interactive resources, ...
- Use both non-code and code examples in class
  - This is important in a CS50 classroom.
  - David Malan will show code examples in lecture, whereas Doug will provide illustrations in shorts to think about concepts differently.
    - For example, to explain stepping into an array, discuss finding mail in post office boxes.
    - The point is to have students see the parallels between the two explanations.
- Before revealing answer, ask for alternative
  - Whether or not students give the right answer in discussion, be sure to field for more solutions from other students.
    - Remember, there's more than one correct solution to a problem.
- After showing answer, ask for alternative solutions
  - Again, there's more than one correct solution to a problem.
- Discuss tradeoffs of different approaches
  - CS50 does this a lot around problem set 3 at Harvard.
    - Searching and sorting algorithms
      - Why is one better than the other?
  - Hash tables vs tries
    - Tries take up more memory.
    - Hash tables take more to search.

### Creating a Culture of ~~Eror~~ Error
- It's important to make mistakes in front of students regularly. This lets students know:
  - It is okay to struggle.
    - Doug gives an anecdote about when he was once a math major at Harvard.
      - He went to office hours with one of his math professors to seek help with a problem.
        - Another student there was clearly understanding the material better than Doug.
        - The professor turned to Doug and said, "He gets this, why don't you get this?"
        - Doug never went to office hours again during his undergrad and changed majors.
    - Students should never feel like that because they don't understand something right away that they are deficient.
  - It is okay to be wrong.
  - Error is respected.
  - Error is normal.
  - Error can be learned from.
- Rather than asking "Does anyone have any questions?", ask "What questions do you have?"
  - "Does anyone have any questions" puts students on the spot.
  - "What questions do you have?" normalizes asking questions.
  - "What other ideas are out there?" is another good question.
- Sometimes more effective to show students an incorrect solution than a correct one.
  - Have students code out of the incorrect solution line by line.
  - Instills skills in debugging.
- Let students figure out your mistake.
  - It's great to wait for students to see your mistake.
- Encourage discussion and guessing.
  - Create a community to foster this.

### Feedback
- It's challenging to teach undergraduate staff how to give quality feedback.
- Not feedback:
  - "You might want to use a for loop instead here."
    - Just projecting an opinion but not defending it.
  - "Design: 3 out of 5"
    - Why was design 3 out of 5?
  - "Great!"
  - These are actually advice and value judgements.
- Feedback in a CS50 Classroom
  - `check50` assesses correctness for you automatically, giving you more time to focus on design.
    - `style50` will likewise grade style automatically.
    - Design is where CS50 focuses qualitative feedback and comments.
  - [CS50.me](https://cs50.me) and GitHub makes it easy to provide detailed comments on specific lines of code, and lets students engage in conversation about their code.
- 7 Keys to Effective Feedback
  - [Article by Grant Wiggins](http://www.ascd.org/publications/educational-leadership/sept12/vol70/num01/Seven-Keys-to-Effective-Feedback.aspx)
    1. Goal-referenced
      - What do students want to get out of the class?
    2. Tangible and transparent
      - Not heavy on technical jargon.
    3. Actionable
      - Students should know their next steps for improvement.
    4. User-friendly
    5. Timely
    6. Ongoing
    7. Consistent
      - Don't contradict previous advice.
  - This is what CS50 staff try to keep in mind when providing feedback to students.

#### Code Commenting Strategies
- Keep on file detailed comments about common mistakes, easy to make note on students' code if you notice similar issues. (GitHub "Saved Replies")
  - Saves time
- For each problem, best to offer multiple pluses and multiple deltas.
  - Pluses: things the student did well
  - Deltas: things the student should change
- Common issues to look for: repetition of code, lack of clarity, more complexity than necessary
  - Best to address these early when programs are smaller.
  - Instill the importance of clarity with variable names.

### Teacher Questions
**Question 1: How do CS50.me and GitHub relate?**
- CS50.me is effectively a frontend for GitHub.
- GitHub saves every version of a problem that a student submits.
- By the end of CS50, students will have a repository full of code.

**Question 2: What about an adopt/adapt hybrid of CS50 AP?**
- This happens a lot.
- Anything that works in your classroom is encouraged.

**Question 3: Does the CS50 IDE work on Android devices and tablets?**
- Yes, it does.
- However, it's not easy to type on phones.

**Question 4: Does CS50 have teachers report student data?**
- CS50 does request demographic information but doesn't require it.

**Question 5: Are prior Puzzle Day questions available online?**
- They are available by request.
- This is so that solutions aren't floating around on the internet.

**Question 6: How long do students have to work on final projects?**
- CS50 at Harvard gives the students 3 weeks.
  - The process involves several milestones:
    - Pre-proposal
    - Proposal
    - Status update
    - Hackathon
    - Submission
- Often projects go beyond the scope of a teacher's knowledge, so teaching students the ability to Google is a must.
  - CS50 seminars can also help with this.

**Question 7: Does CS50 have an AP CSP community in Piazza?**
- No, but CS50 AP has some platforms such as Slack that exist.
- CS50 is looking into a Facebook group for AP students.

**Questions 8: Does the CS50 Hackathon actually have a box of items for set up?**
- Yes, there will be swag giveaways and instructions on how to run the event in the box.
