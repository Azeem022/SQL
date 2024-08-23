use college;  /* which  schema we are working */

create table student (                       /* table creation*/
id int primary key not null,
name varchar(100),
rollno int unique ,
course varchar(100) 
);

select * from student ;           /* Display the table data  */

Insert into student(id ,name , rollno , course )values (1 , "zubair" , 12 ,"b.tech");   /* Insert data in table  */
Insert into student values (2 , "azeem" , 13 ,"b.tech 1st year"); 

update student                /* update column in a table  */
set course ="bba"
where rollno  =13;

delete from student where id =2 ;           /* delete the data from table */
drop table student;                     /* delete the whole table  */


CREATE DATABASE harsh_company;
USE harsh_company;

CREATE TABLE employe(
id INT PRIMARY KEY,
name VARCHAR(50),
salary INT
);

INSERT INTO employe 
(id,name,salary)
VALUES
(1,"MOHD AZEEM",95000),
(2,"MOHD QASIM",96000),
(3,"MOHD KAIF",94000),
(4,"MOHD SHAHZEB",98000);

SELECT * FROM employe;

CREATE TABLE TEMP1(
id INT,
name VARCHAR(50),
AGE INT,
city VARCHAR(50),
PRIMARY KEY (id,name)  /* dono ka combination kabhi same nhi ho skta */
);

CREATE TABLE emp(
id INT ,
salary INT DEFAULT 25000
);

INSERT INTO emp(id) VALUES (101);
SELECT * FROM emp;
/* 
Constraints
CHECK -> column ki values pr limit laga deta hai.
*/

CREATE TABLE city(
age INT CHECK (age >=18)
);

CREATE DATABASE university;
USE university;

CREATE TABLE student(
roll_no INT PRIMARY KEY,
name VARCHAR (50),
marks INT NOT NULL,
grade VARCHAR(1),
city VARCHAR(20)
);

INSERT INTO student 
(roll_nO,name ,marks,grade,city)
VALUES
(11,"MOHD KASIM",85,"B","AMROHA"),
(12,"MOHD AZEEM",86,"B","RAJAKPUR"),
(13,"MOHD KAIF",70,"B","AZAMPUR"),
(14,"MOHD SHAHZEB",60,"B","DHANAURA"),
(15,"MOHD SUHAIB",90,"B","CHANDPUR");

SELECT * FROM student



UPDATE student SET grade = 'A' WHERE roll_no = 15;
UPDATE student SET grade = 'D' WHERE roll_no = 14;
UPDATE student SET grade = 'C' WHERE roll_no = 13;

SELECT * FROM student;
SELECT name,grade FROM student;
SELECT DISTINCT grade FROM student;/* distinct keywords is used to find the data which is not repeated in that row*/
SELECT * FROM student WHERE marks >=80; /* WHERE is used to find some condition */ 
SELECT * FROM student WHERE marks+10 >100;/* yaha hum koi bhi arthmetic operators use kr skte hai*/
SELECT * FROM student WHERE marks >=60 AND CITY = "amroha" OR city= "chandpur";
SELECT * FROM student WHERE marks BETWEEN 70 AND 90;
SELECT * FROM student WHERE city IN ("amroha","azampur");
SELECT * FROM student WHERE city NOT IN ("amroha","azampur");
SELECT * FROM student LIMIT 2;
SELECT * FROM student ORDER BY city ASC;
SELECT * FROM student ORDER BY marks DESC LIMIT 3;
