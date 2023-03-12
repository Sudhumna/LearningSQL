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

 

    

    


