![Logo](images/Logo1.png)
# BA510 Final Project
__Spring 2020__

__By Jessica Veroline and Tetiana Nadkernychna__

---
## 1. ***CourseData*** database creation
- Created a `CourseDataETL.ipynb` journal. 
- [CourseDataERD](http://github.com/fairfield-ba510-spring2020/term-project-jt/blob/master/docs/CourseDataERD.pdf) Displays the information that can be found in our Course Data ERD. 
- We created a design that included the tables with data joined by the foreign keys. The relations were normalized.
- All sourse data was imported into temporary tables.
- The data was then imported into the **CourseData** database. 


[CourseDataETL](https://github.com/fairfield-ba510-spring2020/term-project-jt/blob/master/CourseDataETL.ipynb)

---
## 2. Test of database integrity
- Created a `CourseDataTest.ipynb` journal.
- Tested the entity integrity of the **CourseData** database to ensure that the data was error free. 
- Tested the relational integrity of the **CourseData** database to make sure the tables were correctly formed. 


[CourseDataTest](https://github.com/fairfield-ba510-spring2020/term-project-jt/blob/master/CourseDataTests.ipynb)

---
## 3. ***CourseDataWarehouse*** creation
- Created a `CourseDataWarehouse.ipynb` journal.

- [DataWarehouseERD](https://github.com/fairfield-ba510-spring2020/term-project-jt/blob/master/docs/DataWarehouseERD.pdf) Displays the ERD formed **CourseDataWarehouse**. 
- Using a star schema design, we created a data warehouse: 
  + *Fact* table `CLASS_STATISTICS` represents each class taken from *Fall 2014* to *Spring 2019* and 
  + *Dimention* tabes `TERM1`, `PROGRAM1`, `LOCATION1`, `INSTRUCTOR1`, and `COURSE1` store data about terms, programs, locations, instructors and courses respectively.
- We imported the data from the **CourseData** database into the **CourseDataWarehouse** database. 


[CourseDataWarehouse](https://github.com/fairfield-ba510-spring2020/term-project-jt/blob/master/CourseDataWarehouse.ipynb)

---
## 4. Test of data warehouse integrity
- Created a `CourseDataWarehouseTest.ipynb` journal.
- Tested the entity integrity of the **CourseDataWarehouse** database to ensure that the data was error free. 
- Tested the relational integrity of the **CourseDataWarehouse** database to make sure the tables were correctly joined. 

[CourseDataWarehouseTest](https://github.com/fairfield-ba510-spring2020/term-project-jt/blob/master/CourseDataWarehouseTest.ipynb)

---
## 5. Demonstration of data warehouse queries
- Created a `CourseDataWarehouseDemo.ipynb` journal.

#### Question 1
- ***What was the total number of hours each professor taught during 2018?***
- We thought it could be interesting to see the total number of hours each professor teaches because it could tell us if another professor needs to be hired. If one professor is working more hours than he or she should be, then another professor may need to be hired to make up the difference. 
- When we set the limit to 5, we can already see how *Aaron R. Van Dyke* taught 211 hours while two other professors taught 70 hours. That is a big difference, and it could be that the other two professors are part time or adjunct professors. 

#### Question 2
- ***What was the total number of professors that worked within each program during 2018?*** 
- This could be interesting to see which program is most popular at *Fairfield University*. As the number of students within a program increases, the demand for professors increases as well. 
- When we limit the query to five results, we see that the nursing program has the most professors with 75. Fairfield is known for its nursing school and there are many nursing students who attend the *Fairfield* so it is not very surprising. Programs such as English and science are a requirement for Fairfield’s core curriculum so it is not surprising that those programs are also rather large. 

#### Question 3
- ***What were the most used classrooms in DSB during each term?***
- This query shows how many distinct classes (not meeting times) each *Dolan School of Business* auditorium holds in a given term. 
- With this information we can see how often each room is occupied and should there be additional expansion of the building or if there are rarely occupied rooms that can be used for other purposes.

#### Question 4
- ***What is the student to teacher ratio by program?***
- When evaluating whether or not more faculty should be hired, the University can use this query. It shows the number of students divided by the number of sections for a program. 
- We mainly focused on the business school, but that can easily be changed to evaluate other schools. After running the query, we found that marketing classes tend to have larger class sizes, nearing 30 students per class. As demand increased between 2017 and 2018, we see that the University responded by increasing the number of sections taught. 


[CourseDataWarehouseDemo](https://github.com/fairfield-ba510-spring2020/term-project-jt/blob/master/CourseDataWarehouseDemo.ipynb)


## END.

---