## SQL (Structured Query Language)
SQL is a powerful language that's used for communicating with databases. Every application that manipulates any kind of data
needs to store that data somewhere; whether it's big data,
or just a table with a few simple rows for government, or a small startup, or a big database that spans over multiple servers or a mobile phone that runs its own small database.
### Database
A database is a repository of data. It is a program that stores data.
A database also provides the functionality for adding, modifying, and querying that data. There are different kinds of databases of different requirements.
#### Relational Database
When data is stored in tabular form, the data is organized in tables like in a spreadsheet, which is columns and rows. That's a relational database.
### DBMS &RDBMS
A set of software tools for the data in the database is called a database management system or DBMS for short. The terms database, database server, database system, data server, and database management systems are often used interchangeably. For relational databases, it's called a relational database management system or RDBMS. RDBMS is a set of software tools that controls the data such as access, organization, and storage. And RDBMS serves as the backbone of applications in many industries including banking, transportation, health, and so on. Examples of relational database management systems are my SQL, Oracle Database, DB2 Warehouse, and DB2 on Cloud. For the majority of people using a database, there are five simple commands to create a table, insert data to populate the table, select data from the table, update data in the table, delete data from the table. So those are the building blocks for SQL for data science.
#### Select Statement
The SELECT statement is used to select data from a database.

    SELECT column1, column2, ...
    FROM table_name
    WHERE condition
    ;
    
**What do the keywords / clauses of a SQL statement shown above do?**

-   **FROM**: Specifies from which table to get the data. The clause can include optional JOIN subclauses to specify the rules for joining tables.
-   [Optional Clause]  **WHERE**  : Specifies which rows to retrieve.

  

**Why is there a semicolon after the SQL statements?**

-   Some database systems require a semicolon at the end of each SQL statement for execution. It is a standard way to separate one SQL statement from another which allows more than one SQL statement to be executed in the same call to the server. So, it is good practice to use a semicolon at the end of each SQL statement.

#### Expressions that are used with SELECT statements
**Database:** FilmLocations is given for all these examples.

**COUNT**,   is an aggregate function that retrieves the number of rows that matches the query criteria.

*Retrieve the number of rows from the “FilmLocations” table.*

    SELECT COUNT(*) FROM FilmLocations;

**DISTINCT** is used to remove duplicate values from a specified 
result set and only return the unique values. 

*Retrieve the name of all films without any repeated titles.*

    SELECT DISTINCT Title FROM FilmLocations;

 **LIMIT** is used for restricting the number of rows retrieved from the table.
 
 *Retrieve the first 25 rows from the “FilmLocations” table.*

     SELECT * FROM FilmLocations LIMIT 25;

 ### DML (Data Manipulation Language) statements of SQL

 - **INSERT statement:**

 It is used to insert new rows into a table. 
  
    UPDATE table_name
    SET column1 = value1, column2 = value2, ...
    WHERE condition
    ;
 - **UPDATE statement:**

 It is used to update the data in existing rows in the table. 

    UPDATE table_name
    SET column1 = value1, column2 = value2, ...
    WHERE condition
    ;  
 - **DELETE statement**:

  It is used to remove rows from a    table.

    DELETE FROM table_name
    WHERE condition
    ;
    
![SQL Basic commands](https://raw.githubusercontent.com/Sudhumna/LearningSQL/main/SQL_CHEETSHEET.png)
    
SQL statements fall into two different categories:

Data Definition Language statements and Data Manipulation Language statements.

**Data Definition Language (or DDL)** statements are used to define, change, or drop database objects such as tables.

Common DDL statement types include CREATE, ALTER, TRUNCATE, and DROP.

**CREATE:** which is used for creating tables and defining its columns;

**ALTER:** is used for altering tables including adding and dropping columns and modifying their datatypes;

**TRUNCATE:** is used for deleting data in a table but not the table itself;

**DROP:** is used for deleting tables.

**Data Manipulation Language (or DML)** statements are used to read and modify data in tables. These are also sometimes referred to as CRUD operations, that is, Create, Read, Update and Delete rows in a table.

Common DML statement types include INSERT, SELECT, UPDATE, and DELETE.

**INSERT:** is used for inserting a row or several rows of data into a table;

**SELECT:** reads or selects row or rows from a table.

**UPDATE:** edits row or rows in a table.

 **DELETE:** removes a row or rows of data from a table.

 - *DDL or Data Definition Language statements are used for defining or changing objects in a database such as tables.*
 - *DML or Data Manipulation Language statements are used for manipulating or working with data in tables.*
    


