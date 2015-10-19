# SQL NOTES

## Describe the concept of a database schema
  ### **What are database schemas for?**
  >A SQL scheme is container of objects. For example you may have a large enterprise application and it is good practice to use different schemes for different purposes (e.g. put HR related tables into HR scheme, accounting related tables into Accounting scheme and so on). A schema can be owned by any user, and the ownership is transferable.

  ### **What are some examples of schema modification statements?**

>**DDL** *Data Definition Language (DDL)* statements are used to define the database structure or schema. Some examples:

  - CREATE - to create objects in the database
  - ALTER - alters the structure of the database
  - DROP - delete objects from the database
  - TRUNCATE - remove all records from a table, including all spaces allocated for the records are removed
  - COMMENT - add comments to the data dictionary
  - RENAME - rename an object

>**DML** *Data Manipulation Language (DML)* statements are used for managing data within schema objects. Some examples:

  - SELECT - retrieve data from the a database
  - INSERT - insert data into a table
  - UPDATE - updates existing data within a table
  - DELETE - deletes all records from a table, the space for the records remain
  - MERGE - UPSERT operation (insert or update)
  - CALL - call a PL/SQL or Java subprogram
  - EXPLAIN PLAN - explain access path to data
  - LOCK TABLE - control concurrency

>**DCL** *Data Control Language (DCL)* statements. Some examples:

  - GRANT - gives user's access privileges to database
  - REVOKE - withdraw access privileges given with the GRANT command
TCL

>**TLC** *Transaction Control (TCL)* statements are used to manage the changes made by DML statements. It allows statements to be grouped together into logical transactions.

  - COMMIT - save work done
  - SAVEPOINT - identify a point in a transaction to which you can later roll back
  - ROLLBACK - restore database to original since the last COMMIT
  - SET TRANSACTION - Change transaction options like isolation level and what rollback segment to use

## **Compare and contrast SQL databases and Mongo:**

|                      | Mongo                      | SQL                         |
| :------------------- |:-------------------------- | :-------------------------- |
| TYPE                 | Non-Relational/ No Sql     | Relational                  |
| DATA REPRESENTATION  | collections of JSON documents | tables and rows.         |
| QUERYING             |  object (by passing document - nothing to parse)| strings that are then parsed by the database system |
| RELATIONSHIPS        | multi-dimensional data types: arrays, strings, booleans, etc | JOIN OPERATION |
| TRANSACTIONS         | Single Operations (atomic) | Transactions (atomic)       |
| SCHEMA DEFINITIONS   | Don't need to define (can have different fields) | Requires to define tables and columns before storying anything, and every row in a table must have the same columns |
| SCHEMA DESIGN AND NORMALIZATION | have to use embedding and linking instead of joins and you don't have transactions | not much flexibility when following normalization standards |
| PERFORMANCE          | usually faster then relational databases | database wrapper and index data correctly will result in better performance |
| WHEN SHOULD YOU USE... | Data seems complex to model or de-normalizing your database schema or coding around performance issues or storing serialized arrays or JSON objects, can't pre-define your schema or storying records in the same collection that have different fields | Data structure fits nicely into tables and rows or if you require SQL or transactions |

## Execute SQL through psql or files



## Write basic crud statements in SQL



## Write common select queries



## Describe SQL relational processes



## Write SQL join statements
![](/images/sqljoin.png)


## Choose the right SQL join based on a given problem



## Model one to many and many to many relationships



## Aggregate data in queries



## Describe database permissions




### REFERENCES:
1. [MySql vs MongoDB](http://www.neonrain.com/blog/mysql-vs-mongodb-relational-and-non-relational-databases)
1.  [Difference between DDL, DML and DCL commands.](http://www.ittutorials.in/source/sql/sql-ddl-dml-dcl-commands.aspx)
1. 
