The mid term exams of the students have just completed. Now the marking of the
answer sheets have been started and teachers are asking for a software systems
rather than old pen and paper style of giving marks to students.<br/>
<br/>
Now the main goal for you as software developers is to build a module, using
scala language, that represents the marks of the students in a rigid
systematic way and also design the functionalities to calculate marks, finding
best students etc (requirements declared below)<br/>
<br/>
Use **case** classes to represent the attributes of subjects, student, scorecard
and course. The minimum expected attributes of these entities are-<br/>
<br/>
```
Subject :
	name 				//Subject name
	id				//Subject ID
	maxMarks			//maxMarks for a subject
	obtainedMarks		    //Marks obtained by the student
	
Student :
	name 				//Student Name
	rollNumber			//Class roll number for attendance
	age				//Student Age
	gender				//Gender of student
	enrollemntNumber	    //enrollemntNumber alloted during the admission

Scorecard :
	nameOfStudent		    //Name of student
	rollNumber			//Roll Number (you can add enrol. no. too)
	subject1			//Subject from chosen course
	subject2			//Subject from chosen course
	subject3			//Subject from chosen course
	subject4			//Subject from chosen course
	subject5			//Subject from chosen course
	subject6			//Subject from chosen course
	total				//Total of marks
	percentage			//Percentage of student
	grade				//Grades of the student based on grades

	//Note : The subjects mentioned in the scorecard all should be of type
	//Subject case class, that is, you'll end using case class inside case
	//class

Course :
	name 				//Name of the course
	id 				//ID of the course
	category			//category of the Course (like zoology, physics
					//hons, electrical engg etc)

```
Objective 1:<br/>
<br/>
a)  Create the `trait`'s for defining the functionalities/characterisitics for<br/>
the entitites decared above.<br/>
<br/>
b) Create the **case** classes for all of the entities mentioned above. These case<br/>
classes should extend their respective trait classes. Example, Course can<br/>
be a trait having its methods declared inside it and then define the case<br/>
class for actual course entity that extends that trait and implement the method for<br/>
that particular course.<br/>
<br/>
c) Imlement the methods, defined in the trait, in the case classes.<br/>
<br/>
d) Define the `apply()` methods of the case classes to construct the factory
objects of those classes. For example, define the apply() method of the
Scorecard case class that takes the marks of the subjects (along with student
details) and calculates the total, grades and percentage inside the apply
method and save the values of the those attributes accordingly.
<br/><br/>
e) Define the `unapply()` method of the case classes. Use them in proper
situations, e.g. pattern matching.<br/>
