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


## Execute SQL through psql or files



## Write basic crud statements in SQL



## Write common select queries



## Describe SQL relational processes



## Write SQL join statements



## Choose the right SQL join based on a given problem



## Model one to many and many to many relationships



## Aggregate data in queries



## Describe database permissions
