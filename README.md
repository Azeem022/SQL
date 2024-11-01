###############################################What is Database
The database is a collection of inter-related data which is used to retrieve, insert and delete the data efficiently. It is also used to organize the data in the form of a table, schema, views, and reports, etc.
Using the database, you can easily retrieve, insert, and delete the information.

################################################Database Management System
Database management system is a software which is used to manage the database. For example: MySQL, Oracle, etc are a very popular commercial database which is used in different applications.
DBMS provides an interface to perform various operations like database creation, storing data in it, updating data, creating a table in the database and a lot more.
It provides protection and security to the database. In the case of multiple users, it also maintains data consistency.
database 3
Graph databases are very useful when the database contains a complex relationship and dynamic schema.

It is mostly used in supply chain management, identifying the source of IP telephony.

DBMS (Data Base Management System)
Database management System is software which is used to store and retrieve the database. For example, Oracle, MySQL, etc.; these are some popular DBMS tools.

DBMS provides the interface to perform the various operations like creation, deletion, modification, etc.
DBMS allows the user to create their databases as per their requirement.
DBMS accepts the request from the application and provides specific data through the operating system.
DBMS contains the group of programs which acts according to the user instruction.
It provides security to the database.

###########Characteristics of DBMS
DBMS contains automatic backup and recovery procedures.
It contains ACID properties which maintain data in a healthy state in case of failure.
It is used to provide security of data.
It can view the database from different viewpoints according to the requirements of the user.

#########Advantages of DBMS
Controls database redundancy: It can control data redundancy because it stores all the data in one single database file and that recorded data is placed in the database.
Data sharing: In DBMS, the authorized users of an organization can share the data among multiple users.
Easily Maintenance: It can be easily maintainable due to the centralized nature of the database system.
Reduce time: It reduces development time and maintenance need.
Backup: It provides backup and recovery subsystems which create automatic backup of data from hardware and software failures and restores the data if required.
multiple user interface: It provides different types of user interfaces like graphical user interfaces, application program interfaces

#######################Disadvantages of DBMS
Cost of Hardware and Software: It requires a high speed of data processor and large memory size to run DBMS software.
Size: It occupies a large space of disks and large memory to run them efficiently.
Complexity: Database system creates additional complexity and requirements.
Higher impact of failure: Failure is highly impacted the database because in most of the organization, all the data stored in a single database and if the database is damaged due to electric failure or database corruption then the data may be lost forever.

###################What is Data?
Data is a collection of a distinct small unit of information. It can be used in a variety of forms like text, numbers, media, bytes, etc. it can be stored in pieces of paper or electronic memory, etc.

Word 'Data' is originated from the word 'datum' that means 'single piece of information.' It is plural of the word datum.


##################Hierarchical Data Model
1968-1980 was the era of the Hierarchical Database. Prominent hierarchical database model was IBM's first DBMS. It was called IMS (Information Management System).


###########################Relational Database
1970 - Present: It is the era of Relational Database and Database Management. In 1970, the relational model was proposed by E.F. Codd.

Relational database model has two main terminologies called instance and schema.

The instance is a table with rows or columns

Schema specifies the structure like name of the relation, type of each column and name.

###########################The Object-Oriented Databases
The object-oriented databases contain data in the form of object and classes. Objects are the real-world entity, and types are the collection of objects. An object-oriented database is a combination of relational model features with objects oriented principles. It is an alternative implementation to that of the relational model.

Object-oriented databases hold the rules of object-oriented programming. An object-oriented database management system is a hybrid application.

The object-oriented database model contains the following properties.

Object-oriented programming properties

Objects
Classes
Inheritance
Polymorphism
Encapsulation


#############################DBMS (Data Base Management System)
Database management System is software which is used to store and retrieve the database. For example, Oracle, MySQL, etc.; these are some popular DBMS tools.

DBMS provides the interface to perform the various operations like creation, deletion, modification, etc.
DBMS allows the user to create their databases as per their requirement.
DBMS accepts the request from the application and provides specific data through the operating system.
DBMS contains the group of programs which acts according to the user instruction.
It provides security to the database.


#################################RDBMS (Relational Database Management System)
The word RDBMS is termed as 'Relational Database Management System.' It is represented as a table that contains rows and column.

RDBMS is based on the Relational model; it was introduced by E. F. Codd.

A relational database contains the following components:

Table
Record/ Tuple
Field/Column name /Attribute
Instance
Schema
Keys
An RDBMS is a tabular DBMS that maintains the security, integrity, accuracy, and consistency of the data.
A relational database is the most commonly used database. It contains several tables, and each table has its primary key.

Due to a collection of an organized set of tables, data can be accessed easily in RDBMS.

##################################What is table/Relation?
Everything in a relational database is stored in the form of relations. The RDBMS database uses tables to store data. A table is a collection of related data entries and contains rows and columns to store data. Each table represents some real-world objects such as person, place, or event about which information is collected. The organized collection of data into a relational table is known as the logical view of the database.


#####################What is a row or record?
A row of a table is also called a record or tuple. It contains the specific information of each entry in the table. It is a horizontal entity in the table. For example, The above table contains 5 records.

Properties of a row:

No two tuples are identical to each other in all their entries.
All tuples of the relation have the same format and the same number of entries.

#########################What is a column/attribute?
A column is a vertical entity in the table which contains all information associated with a specific field in a table. For example, "name" is a column in the above table which contains all information about a student's name.

Properties of an Attribute:

Every attribute of a relation must have a name.
Null values are permitted for the attributes.
Default values can be specified for an attribute automatically inserted if no other value is specified for an attribute.
Attributes that uniquely identify each tuple of a relation are the primary key.

##########################Data Integrity
There are the following categories of data integrity exist with each RDBMS:

Advertisement

Entity integrity: It specifies that there should be no duplicate rows in a table.

Domain integrity: It enforces valid entries for a given column by restricting the type, the format, or the range of values.

Referential integrity specifies that rows cannot be deleted, which are used by other records.

User-defined integrity: It enforces some specific business rules defined by users. These rules are different from the entity, domain, or referential integrity.
The order of the tuple is irrelevant. They are identified by their content, not by their position.
