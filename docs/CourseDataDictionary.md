![Logo](images/Logo1.png)
# BA510 Final Project
__Spring 2020__

__By Jessica Veroline and Tetiana Nadkernychna__


## Fairfield University Course Catalog Database ERD


![ERD](images/CourseDataERD.png)

## Class
|Name             | Description                                        |
|:----------------|:---------------------------------------------------|
|**`Class_id`**   | a unique identifier for each class                 |
|*`Instructor_id`*| a unique identifier for each instructor            |
|*`Course_id`*    | a unique identifier for each course                |
|`Section`        | an identifier for each section                     |
|`crn`            | an identifier for each course registration number  |
|`Term`           | an identifier for each term                        |
|`Cap`            | the max number of students the class can hold      |
|`Act`            | the number of students in the class                |
|`Rem`            | the number of spots available in the class         |
|`TimeCode`       | when the class takes place                         |

## Meeting
|Name              | Description                                       |
|:-----------------|:--------------------------------------------------|
|**`Meetings_id`** |a unique identifier for the meeting                |
|*`Class_id`*      |a unique identifier for each class                 |
|*`Location_id`*   |a unique identifier for each location              |
|`Start`           |the time that the class begins                     |
|`End`             |the time that the class finishes                   |
|`Day`             |the day of the week that the class meets           |

## Location
|Name              | Description                                           |
|:-----------------|:------------------------------------------------------|
|**`Location_id`** | a unique identifier for each class                    |
|`Location`        |the room and the building in which a class is held         |

## Instructor
|Name                | Description                                                    |
|:-------------------|:---------------------------------------------------------------|
|**`Instructor_id`** | a unique identifier for each instructor                        |
|`Name`              | the name of the instructor                                     |
|`Phone`             |the instructor’s phone number                                   |
|`Email`             |the instructor’s email                                          |
|`Colledge`          |the college that the instructor works for within the University |

## Course
|Name                | Description                                                                    |
|:-----------------|:---------------------------------------------------------------------------------|
|**`Course_id`**   | a unique identifier for each course                                              |
|*`Program_id`*    |a unique identifier for each program                                              |
|`Catalog_year`    |catalog year                                                                      |
|`CatalogID`       |the ID of the course in the catalog                                               |
|`Course_title`    |the name of the course                                                            |
|`Description`     |an explanation what the course entails                                            |
|`Credits`         |the number of credits that a student will earn from taking the course             |
|`Attributes`      |characteristics of the course                                                     |
|`Prerequisites`   |the requirements that must be met in order for a student to qualify for a course  |
|`Corequisites`    |the requirements that should be met at the same time as the course                |
|`Fees`            |any amount of money that must be paid in order to complete the course             |

## Program
|Name             | Description                                            |
|:----------------|:-------------------------------------------------------|
|**`Program_id`** |a unique identifier for each program                    |
|`Program_code`   |the code of the program in which a course falls under   |
|`Program_name`   |the name of the program in which a course falls under   |