# BA510 Final Project
__Spring 2020__
__By Jessica Veroline and Tetiana Nadkernychna__

![Logo](docs/images/logo.png)

## The ERD for the Fairfield University Course Catalog Database

![ERD](docs/images/MoviesTonightERD.png)
## Class
- ‘Class_id’: a unique identifier for each class 
- ‘Course_id’: a unique identifier for each course
- ‘Section_id’: a unique identifier for each section
- ‘Term_id’: a unique identifier for each term
- ‘Instructor_id’: a unique identifier for each instructor
- ‘Cap’: the max number of students the class can hold
- ‘Act’: the number of students in the class
- ‘Rem’: the number of spots available in the class
- ‘Timecode’: When the class takes place

## Meeting
- ‘Meetings_id’: a unique identifier for the meeting 
- ‘Class_id’: a unique identifier for each class
- ‘Location_id’: a unique identifier for each location
- ‘Start’: the time that the class begins 
- ‘End’: the time that the class finishes
- ‘Day’: the day of the week that the class meets

## Location
- ‘Location_id’: a unique identifier for each class
- ‘Capacity’: the maximum number of classes that a building can hold
- ‘Building’: the building in which a class is held
- ‘Room’: the room in which a class is held

## Instructor
- ‘Instructor_id’: a unique identifier for each instructor
- ‘Name’: the name of the instructor
- ‘Phone’: the instructor’s phone number
- ‘Email’: the instructor’s email
- ‘College’: the college that the instructor works for within the University

## Course
- ‘Course_id’: a unique identifier for each course
- ‘Program_id’: a unique identifier for each program
- ‘Term_id’: a unique identifier for each term
- ‘Course_title’: the name of the course
- ‘Description’: an explanation what the course entails
- ‘Credits’: the number of credits that a student will earn from taking the course
- ‘Attributes’: characteristics of the course
- ‘Prerequisites’: the requirements that must be met in order for a student to qualify for a course
- ‘Corequisites’: the requirements that should be met at the same time as the course
- ‘Fees’: any amount of money that must be paid in order to complete the course

## Program
- ‘Program_id’: a unique identifier for each program
- ‘Program_name’: the name of the program in which a course falls under
