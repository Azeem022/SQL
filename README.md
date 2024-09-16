[10:35 pm, 16/9/2024] Azeem Saifi: CREATE DATABASE college_1;
USE college_1;

CREATE TABLE student_1(
Roll_no numeric,
Name CHAR(20),
age INT,
address VARCHAR(30),
date_of_birth DATE,
contact_no NUMERIC(10));

DESC student_1;

INSERT INTO student_1
(Roll_no, Name, age, address, date_of_birth, contact_no)
values
(01, "Aaditya", 12 ,"Moradabad","2004-01-01",9084353600);
INSERT INTO student_1
(Roll_no, Name, age, address, date_of_birth, contact_no)
values
(01, "Aaditi", 15 ,"Delhi","2008-02-18",9084353611);
INSERT INTO student_1
(Roll_no, Name, age, address, date_of_birth)
values
(02, "Aaditi", 17 ,"Moradabad","2004-01-08");
INSERT INTO student_1
(Roll_no, Name, age, address, date_of_birth, contact_no)
values
(01, "Aaditya", 17 ,"Moradabad","2004-01-01",9084353600);
INSERT INTO student_1
(Roll_no, Name, age, address, date_of_birth, contact_no)
values
(05, "Azeem", 17 ,"Amroha","2004-04-04",9084353645);

SELECT * FROM student_1;
[12:07 am, 17/9/2024] Azeem Saifi: CREATE TABLE student_2(
Roll_no INT PRIMARY KEY,
Name  VARCHAR(20) NOT NULL,
Age INT Check(Age>=18),
Address VARCHAR(30),
Date_Of_Birth DATE,
Contact_no NUMERIC(10) UNIQUE
);

DESC student_2;

INSERT INTO student_2
(Roll_no, Name, Age, Address, Date_Of_Birth, Contact_no)
VALUES
(01, "Azeem", 20, "Amroha", "2003-04-12", 8287098601);
INSERT INTO student_2
(Roll_no, Name, Age, Address, Date_Of_Birth, Contact_no)
VALUES
(02, "Asim", 25, "Pakbada", "2004-05-13", 8287098600);
INSERT INTO student_2
(Roll_no, Name, Age, Address, Date_Of_Birth, Contact_no)
VALUES
(03, "Kasim", 24, "Amroha", "2005-05-15", 6398083537);
INSERT INTO student_2
(Roll_no, Name, Age, Address, Date_Of_Birth, Contact_no)
VALUES
(04, "Kaif", 23, "Rajakpur", "2006-06-16", 9568711709);
INSERT INTO student_2
(Roll_no, Name, Age, Address, Date_Of_Birth, Contact_no)
VALUES
(05, "suhaib", 21, "Rajakpur", "2007-07-17", 7253062912);

SELECT * FROM student_2;

SELECT * FROM student_2 

WHERE Address = "Amroha";

SELECT * FROM student_2 

WHERE Roll_no = 3;

ALTER TABLE student_2 ADD Year_Of_Addmission date;

ALTER TABLE student_2 ADD Course char(20) default "BTECH(CS)";

ALTER TABLE student_2 MODIFY Course varchar(20);

ALTER TABLE student_2 drop column Year_Of_Addmission;

UPDATE student_2 SET Address = "Noida", Contact_no = 9568756299 WHERE ROll_no = 1;

UPDATE student_2 SET Name = "Shahzeb", Address = "Ghaziabad", Course = "BTECH(AI)" WHERE Roll_no = 4;

DELETE FROM student_2 WHERE Roll_no = 5;

DELETE FROM student_2 WHERE Roll_no = 4 and Address = "Ghaziabad";

SELECT Roll_no , Name FROM student_2;

desc student_2;

select * from student_2;
