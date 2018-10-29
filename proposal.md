# X-Team 126 Class Enrollment Waitlist 

See https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#code for tips on using *Markdown* tags to format __.md__ files

## Goal

Work as a team to create a project proposal for your X-team to complete together.
The project does not have to be extremely difficult,
but there must be work to do for each member of your team.
You may reference figures using "See figure 1".  
Be sure to submit corresponding image files, i.e. figure1.png (or figure1.jpg) for each figure.

## Grading: To earn full credit, your team's proposal must include:

* (md) documentation: [this file] describing purpose and use of your program

* Description of a program that has:

  ** a main Java program class in a file named Main.java
  
  ** a custom data structure designed and built by your team
  
  ** comprehensive testing of individual units
  
 Caution: You are not being asked to implement this program, at least not yet. 
 We just want your group to make a proposal or pitch for your program.
 
 Tip: Your custom data structure can be composed of or extensions of data structures that you have learned and used in previous programming assignments.  We're looking for decisions about how to build a high-level data structure that will likely have lower-level components.

## Problem Description

We are using queue in order to efficiently manage the waitlist of students who are trying to enroll in CS400 Spring 2019 class. 

## Questions to answer for Exercise #2

1. Name: Give your project proposal a name (and edit the top line of this file)
 Class Enrollment Waitlist


2. Output: Describe the output your program will produce.  Include and example format of the output produced.
The program automatically enrolls the student next in line, as soon as other studenst who has already enrolled drop out. Keeps track of the order of students in the Queue and do not let it go out of capacity. 
Let's suppose there are four students in the waitlist at this moment. Student A was the  first to be on the waitlist, then came student B, and C and D respectively. Then as an enrolled students drops out, student A will automatically be enrolled in the class. After that, if any spot opens up B will automatically get enrolled before C and D. In general, it follows, first in first out strategy. Throws an exception if a student is not elligible to take the class. Also, we can give an update to the students about the size of the queue so that they can decide wheather they want to stay on or find another class. 


3. Input: Describe the data that is needed to solve your problem. Include an example format of the input data.
The data required are as follows:
a. Identity of a student. (Name, Student ID, DOB, school year, etc)
b. Date and time they got added to the queue. 
c. Met cerain conditions or not ( pre req, year in school)
NOTE: Students have authority to add and delete themselves from te waitlist by going into the course website and filling out a simple form.

4. User Interface: Describe a user interface for your program.  Use text menus or a simple graphic user interface.
Text menus to let students check their status in the waitlist, and give them a general idea if they should keep waiting or find another class. Students who wish to add them into the waitlist they can do so by filling out a form online in school website. 


5. Types List: Break your solution idea down into units that you think can be implemented with a single class.

** queueADT --> the interface with usual queue method such as enqueue, dequeue, peek, isEmpty. 

** Node class ( each student is a node and their personal informatino is stored there)
 This class should have most of the required methods including enqueue, dequeue, peek, isempty, etc. And, we add the method that checks if the student no longer wishes to be on the waitlist and remove them accordingly. Also, a method to automate the process of enrolling a waitlist student as soon as there a spot open. finally, we can add a method to keep track of number of students in the class, maxximum capacity, and number of students in the waitlist and autmatically informs them about their status.  A new node is constructed when a student adds their information on the class webiste.
 

Name each interface or class and briefly describe its function or purpose.



## Edit and Submit this file and any figures referenced by this document.

