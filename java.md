# Week 6

* [Method Signatures](https://docs.oracle.com/javase/tutorial/java/javaOO/methods.html)
* [Method Overloading](https://www.geeksforgeeks.org/overloading-in-java/)
* [Last Week's code](https://github.com/GedMullen/java/tree/master/week5/inheritance)
* [Updated Class Diagram](https://drive.google.com/open?id=1ZkLt18MFh-12Yz8gUAlamMRUYusF0KAr)

## Exercises
* Update the code to add the "Person has an Address" relationship. Pass the address into the constructor of the Person object.
* You may not have the address of all Staff/Students. Add in an overloaded constructor to allow for this.
<!--
* Expand the application to have a menu with the following options:
	* Search for person.
	* Add Student. 
-->
# Week 5

* [Inheritance Tutorial](https://www.tutorialspoint.com/java/java_inheritance.htm)
* [Submission](http://moodle.forthvalley.ac.uk/moodle/mod/assign/view.php?id=81694&group=2463)
* [Abstraction - Generalisation](https://docs.google.com/presentation/d/1ayqwPLIqOVPmjWP3LclbivWFTwE1syGoCxLnR9zdVtY/edit?usp=sharing)
* [Java Dates And Times](http://www.tutorialspoint.com/java/java_date_time.htm)
* [Exceptions Tutorial](https://www.tutorialspoint.com/java/java_exceptions.htm)
* [UML Class Diagrams](https://drive.google.com/file/d/0B-CFaefA1v4RTmhRa2NEUHpFcXc/view?usp=docslist_api)
* [Access (Visibility) Modifiers](https://docs.oracle.com/javase/tutorial/java/javaOO/accesscontrol.html)
* [OOP Key Principles - Encapsulation](https://docs.google.com/presentation/d/1iY-umOTsc66EythgwvxxafqMDW4UDYRfrOUq0FN2Vzo/edit?usp=sharing)
## Exercise

* Implement this [class diagram](https://docs.google.com/presentation/d/1ayqwPLIqOVPmjWP3LclbivWFTwE1syGoCxLnR9zdVtY/edit#slide=id.p6). Create a Controller class that instantiates instances of Student and Staff and outputs the contents of the object to the console (override toString()). Set the type of the dateOfBirth attribute should a String.
* Change the dateOfBirth attribute to type Date. Parse the date string passed into the constructor to create a Date attribute.
* Create an ArrayList of Students and an ArrayList of Staff. Modify your Controller to prompt for a name and search through each of the ArrayLists to see if there is a match. Output an appropriate message.
* Modify the code above to use only one ArrayList.
Create two subclasses of Staff - Lecturer and Management. Lecturers have an additional attribute "subjectSpeciality" and managers have an additional attribute "department".
<!--
-->

# Week 4

* [OOP Key Principles - Abstraction](https://docs.google.com/presentation/d/1mgbg_7FeEMJJeu2vH_Y8Kll8ufKYG3qWAFFGIWKBHMI/edit?usp=sharing)
* [Arrays](https://www.tutorialspoint.com/java/java_arrays.htm)
* [Array Lists](https://www.javatpoint.com/java-arraylist)
* [Iterating Through ArrayList](https://gist.github.com/GedMullen/9223ae030ff1c9c5e99318279fc91452)
* [Oracle Certification](https://education.oracle.com/oracle-certification-exams-list)
<!--
* [Warm Up Answers](https://github.com/GedMullen/java/tree/master/warmup5-11)
* [OOP Key Principles - Encapsulation](https://docs.google.com/presentation/d/1iY-umOTsc66EythgwvxxafqMDW4UDYRfrOUq0FN2Vzo/edit?usp=sharing)
-->
## Exercises

* Modify the Controller.java to check for the username "admin" and password "password". Output a successful login message if the user enters the correct username/password combination.
* Create a menu that allows the user to execute each of the warmup exercises.
<!--
* Look at the [Warm Up Answers](https://github.com/GedMullen/java/tree/master/warmup5-11). Can you make any improvements?
-->
* Create a "Course" class that contains a course name (String) and a collection of of student names (ArrayList<String>). Populate the ArrayList with students and print out the array list in your main method.
* Create a Controller class that allows the user to enter the name of a student. If the student is on the course the program should display the message "the student is on the course" otherwise the message "the student is not on the course" should be output to the console.

# Week 3
 
* [Use Case Intro](https://docs.google.com/presentation/d/12LguEoxFnRpudMGFXiUSkXRO3o7nGsrYpSoqGFaFU08/edit?usp=sharing)
* [Use Case Descriptions](https://docs.google.com/presentation/d/1oa1b0NyJd6A_mF2GCjdBbE8dqmzzHVtMmXDHXEV-Me8/edit?usp=sharing)
* [Use Cases Tutorial](http://www.usability.gov/how-to-and-tools/methods/use-cases.html)
* [Agile Use Case Tutorial](http://www.agilemodeling.com/artifacts/useCaseDiagram.htm)
* [Ch3 UML Distilled Use Cases](http://www.amazon.co.uk/UML-Distilled-Standard-Modeling-Technology/dp/0321193687)
* [Draw.io](https://www.draw.io/)
* [Vending Machine Description](https://docs.google.com/document/d/1Eucn9fDemkJmoLM0xtM92mou7vyhWIxCouGaYu0PQP8/edit?usp=sharing)
* [Deadlines](https://docs.google.com/spreadsheets/d/1k4FEsRQcoX1WEdatdkQ17lrfx29YZ539LxWIM1QuJIs/edit?usp=sharing)

## Exercises

* Complete the [Use Cases Tutorial](http://www.usability.gov/how-to-and-tools/methods/use-cases.html)   
* Review the [Agile Use Case Tutorial](http://www.agilemodeling.com/artifacts/useCaseDiagram.htm)
* In your groups think about the process of paying for shopping using a self service checkout at a supermarket. Write the main success scenario for this process. Create a Google Slide to demonstrate your use case description. Make sure you include the precondition and trigger for the scenario.
* Create an alternative path/scenario for a shopping basket that includes alcohol.
* Create an exceptional flow for the above scenario.
* Create a separate Use Case that details the process of a checkout assistant checking the amount of money in the self service machine.
* Create a System Level Use Case diagram for the two use cases above using draw.io.
* Identify 4 other Use Cases associated with a computer system that serves a supermarket. Draw a system level use case diagram that shows these scenarios. 

# Week 2

* [Oracle OOP Introduction](https://docs.oracle.com/javase/tutorial/java/concepts/index.html)
* [OOP Tutorial](https://www3.ntu.edu.sg/home/ehchua/programming/java/J3a_OOPBasics.html).
* [Coding Standards](http://www.asch.org.uk/programming/general/standards.html)
* Answers to warm up exercises 1-4 using [Cloud Shell](https://console.cloud.google.com/cloudshell/):
```bash
mkdir week2
cd week2
git clone https://github.com/GedMullen/java.git
cd java/warmup1-4
javac Exercises.java
java Exercises
```
* [Warm Up Exercise Answers 1-4](https://github.com/GedMullen/java/blob/master/warmup1-4/Exercises.java)
* Console input:
```bash
cd java\intro
javac Controller.java
java Controller
```

## Exercises

* In your groups identify a real world object (e.g. Person) and describe the following:
	* State attributes of the object (e.g. Brown Eyes)
	* Behavioural aspects of the object (e.g. Talks)
	* Name an "is a" relationship of the object (e.g. Animal)
	* Name a sub class (e.g. Female)
* Complete the [Oracle OO Introduction](https://docs.oracle.com/javase/tutorial/java/concepts/index.html)
* In your groups create a 10 minute presentation that answers the following questions:
	* What is OOP - What are its key concepts?
	* What are the advantages of OOP over procedural programming?
	* Explain the term "Instantiating an object in Java" -  provide a code example.
* Start working through the [OOP Tutorial](https://www3.ntu.edu.sg/home/ehchua/programming/java/J3a_OOPBasics.html).
* Modify Controller.java to check for the username "admin" and password "password". Output a successful login message if the user enters the correct username/password combination.
* From the Controller class instantiate an instance of Exercises if the user logs in correctly and call all the methods in Exercises. 


# Week 1

* [Corners Game](https://docs.google.com/document/d/1f8YCnRpKR5dgO-aP77ZXJg5SU6BWLMkiLsc99n1WZe4/pub)
* [Getting Started With Cloud Shell](https://cloud.google.com/shell/docs/starting-cloud-shell)
* [Learning the Command Line on Codecademy](https://www.codecademy.com/learn/learn-the-command-line)
* [The Art Of The Command Line](https://github.com/jlevy/the-art-of-command-line)
* [Units Introduction](https://docs.google.com/presentation/d/1vjJw28aysAXbqeHky2WEMIa-3JgJyaB9voCqvJ-3qYQ/edit?usp=sharing)
* [GitHub Is Your New CV](http://code.dblock.org/2011/07/14/github-is-your-new-resume.html)
* [GitHub Home](https://github.com/)
* [Example Profile](https://github.com/marijnh)
* [Mineplex Project Contributions](https://drive.google.com/file/d/0B7l9n3yk5ob0b0JCWXU5ZjY4dUk/view?ts=58170cea)
* [The mind behind Linux | Linus Torvalds](https://www.youtube.com/watch?v=o8NPllzkFhE)
* Unit Descriptors: [H17135](http://www.sqa.org.uk/files/hn/H17135.pdf) and  [H17235](http://www.sqa.org.uk/files/hn/H17235.pdf)
* [Oracle Java Tutorial](https://docs.oracle.com/javase/tutorial/)
* Running Java in Cloud Shell:
```bash
mkdir week1
cd week1
git clone https://github.com/GedMullen/java.git
cd java/intro
javac HelloWorld.java
java HelloWorld
```

## Exercises

<BR>1 . Complete the [Getting Started With Cloud Shell](https://cloud.google.com/shell/docs/starting-cloud-shell) tutorial.
<br>2 . Complete the [Learning the Command Line on Codecademy](https://www.codecademy.com/learn/learn-the-command-line) course.
<br>3 . Create a GitHub accound and Complete these [GitHub Exercises](https://docs.google.com/document/d/1lYOmyY0liBNXntOP9yipcD7Cy-aqKqAU1gkrSmdd2e4/edit?usp=sharing)
<br>4 . Complete the following warm up [exercises.](https://docs.google.com/document/d/1xrO981Us1UyecvPCDTqdcVK8JynzlbnyNY1Hew8WuRY/edit?usp=sharing)


