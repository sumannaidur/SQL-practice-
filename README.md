# SQL Notes for Freshers

## 1. Introduction to SQL

### • What is SQL?

* **Subtopics:**
    * Definition: Structured Query Language
    * Purpose: Managing and manipulating relational databases
    * Pronunciation: "Sequel" or "Ess-Q-L"
* **HackerRank Questions:** (Conceptual, not direct coding)
    * None directly, but understanding the basics is crucial for all other problems.
* **Interview Questions:**
    1. What does SQL stand for?
    2. Explain in your own words what SQL is used for.
    3. Is SQL a programming language? Why or why not?
    4. What is the primary goal of SQL?
    5. Can you name a few popular Relational Database Management Systems (RDBMS) that use SQL?
    6. What is the difference between SQL and a database?
    7. Why is SQL so widely used in the industry?
    8. What are the main categories of SQL commands?
    9. Briefly describe the client-server architecture in the context of SQL.
    10. What are the advantages of using SQL?

### • Features and Uses of SQL

* **Subtopics:**
    * Data retrieval
    * Data manipulation (insert, update, delete)
    * Data definition (create, alter, drop tables)
    * Data control (permissions)
    * Transaction control
    * Used in Web Development, Data Analysis, Business Intelligence, etc.
* **HackerRank Questions:** (Conceptual, not direct coding)
    * Any basic SELECT, INSERT, UPDATE, DELETE problem implicitly tests understanding of these uses.
* **Interview Questions:**
    1. List three key features of SQL.
    2. How is SQL used in a typical web application?
    3. Can SQL be used for data analysis? How?
    4. What is the role of SQL in Business Intelligence?
    5. Beyond storing data, what else can SQL help you achieve?
    6. Give an example of how SQL ensures data integrity.
    7. How does SQL facilitate concurrent access to data?
    8. What are the benefits of using a standardized language like SQL?
    9. Can SQL interact with other programming languages? Give an example.
    10. How does SQL help in managing large datasets?

### • History of SQL

* **Subtopics:**
    * Developed by IBM in the 1970s (System R project)
    * Originally called SEQUEL (Structured English Query Language)
    * First commercial product: Oracle (1979)
    * ANSI standardization
* **HackerRank Questions:** (Conceptual)
    * None.
* **Interview Questions:**
    1. When and where was SQL originally developed?
    2. What was SQL initially called?
    3. Which company was instrumental in the early development of SQL?
    4. When did SQL become an ANSI standard?
    5. Why was it important for SQL to become a standard?
    6. Name one significant milestone in the history of SQL.
    7. How has SQL evolved since its inception?
    8. Which RDBMS was one of the first to implement SQL commercially?
    9. What problem was SQL trying to solve when it was first created?
    10. How does the history of SQL relate to its current widespread use?

### • SQL Standards (ANSI)

* **Subtopics:**
    * American National Standards Institute (ANSI)
    * Ensures compatibility and portability across different RDBMS
    * Different versions (SQL-92, SQL:1999, SQL:2003, etc.)
* **HackerRank Questions:** (Conceptual)
    * None directly, but knowing standards helps in understanding general syntax.
* **Interview Questions:**
    1. What is the role of ANSI in SQL?
    2. Why is SQL standardization important?
    3. Does every RDBMS fully adhere to ANSI SQL standards? Explain.
    4. What are the advantages of writing standard SQL code?
    5. Name a common difference you might find between different RDBMS implementations of SQL despite standardization.
    6. How does SQL standardization benefit developers?
    7. What does it mean for SQL to be "portable"?
    8. Are there any disadvantages to SQL standardization?
    9. How often are new SQL standards released?
    10. What is a "vendor-specific extension" in the context of SQL?

### • SQL Syntax Basics

* **Subtopics:**
    * Statements end with a semicolon (`;`)
    * Case insensitivity (keywords vs. identifiers)
    * Comments (`--` for single line, `/* ... */` for multi-line)
    * Keywords (SELECT, FROM, WHERE, etc.)
    * Identifiers (table names, column names)
* **HackerRank Questions:**
    * [Revising the Select Query I](https://www.hackerrank.com/challenges/revising-the-select-query/problem)
    * [Revising the Select Query II](https://www.hackerrank.com/challenges/revising-the-select-query-2/problem)
    * [Select All](https://www.hackerrank.com/challenges/select-all-from-table/problem)
    * [Select By ID](https://www.hackerrank.com/challenges/select-by-id/problem)
* **Interview Questions:**
    1. What is the significance of the semicolon at the end of a SQL statement?
    2. Is SQL case-sensitive? Explain.
    3. How do you add a single-line comment in SQL?
    4. How do you add a multi-line comment in SQL?
    5. What is the difference between a SQL keyword and an identifier?
    6. Can you use spaces in table or column names? If so, what are the best practices?
    7. What is the general structure of a basic SELECT statement?
    8. Why is it important to follow consistent naming conventions for identifiers?
    9. Give an example of a simple SQL statement.
    10. What are some common pitfalls for beginners regarding SQL syntax?

## 2. Datatypes

### • Numeric Types (INT, FLOAT, DOUBLE, etc.)

* **Subtopics:**
    * `INT` (INTEGER): Whole numbers (e.g., `TINYINT`, `SMALLINT`, `MEDIUMINT`, `BIGINT`)
    * `DECIMAL`/`NUMERIC`: Exact numeric values (precision and scale)
    * `FLOAT`/`REAL`: Single-precision floating-point numbers
    * `DOUBLE`/`DOUBLE PRECISION`: Double-precision floating-point numbers
* **HackerRank Questions:** (Implicitly used in many problems)
    * Many problems involve numerical comparisons and calculations, requiring an understanding of numeric types. For instance, any problem involving sums, averages, or specific numerical conditions.
* **Interview Questions:**
    1. What is the primary difference between `INT` and `FLOAT` data types?
    2. When would you use `DECIMAL` instead of `FLOAT` or `DOUBLE`?
    3. Explain `precision` and `scale` in the context of `DECIMAL`.
    4. Which numeric datatype would you choose for storing a person's age, and why?
    5. Which numeric datatype is best suited for storing monetary values? Justify your answer.
    6. What is the range of values for `TINYINT`?
    7. Can you store negative numbers using `UNSIGNED INT`?
    8. What are the potential issues with using `FLOAT` for calculations that require exact precision?
    9. If you need to store very large integer values, which datatype would you choose?
    10. How does a database handle overflow errors with numeric types?

### • String Types (CHAR, VARCHAR, TEXT)

* **Subtopics:**
    * `CHAR(n)`: Fixed-length string (padded with spaces)
    * `VARCHAR(n)`: Variable-length string
    * `TEXT`: Large text blocks (e.g., `TINYTEXT`, `MEDIUMTEXT`, `LONGTEXT`)
    * `BLOB`: Binary Large Object (for binary data like images)
* **HackerRank Questions:** (Implicitly used in many problems)
    * [Weather Observation Station 6](https://www.hackerrank.com/challenges/weather-observation-station-6/problem) (involves string matching)
    * [Weather Observation Station 7](https://www.hackerrank.com/challenges/weather-observation-station-7/problem)
    * [Weather Observation Station 8](https://www.hackerrank.com/challenges/weather-observation-station-8/problem)
* **Interview Questions:**
    1. What is the key difference between `CHAR` and `VARCHAR`?
    2. When would you prefer to use `CHAR` over `VARCHAR`? Provide an example.
    3. If you store a 5-character string in a `CHAR(10)` column, how much space does it consume? What about `VARCHAR(10)`?
    4. What is the maximum length of `VARCHAR`? (Note: Varies by RDBMS)
    5. When would you use a `TEXT` datatype instead of `VARCHAR`?
    6. What is `BLOB` used for?
    7. Are string comparisons case-sensitive in SQL by default? How can you change this behavior?
    8. What happens if you try to insert a string longer than the defined length of a `VARCHAR` column?
    9. What are the performance implications of choosing `CHAR` vs. `VARCHAR` for frequently updated columns?
    10. How do different character sets affect string data types?

### • Date & Time Types (DATE, DATETIME, TIMESTAMP)

* **Subtopics:**
    * `DATE`: Stores date only (YYYY-MM-DD)
    * `TIME`: Stores time only (HH:MM:SS)
    * `DATETIME`: Stores date and time (YYYY-MM-DD HH:MM:SS)
    * `TIMESTAMP`: Stores date and time, often with timezone awareness, automatically updated
    * `YEAR`: Stores a year
* **HackerRank Questions:**
    * [The Report](https://www.hackerrank.com/challenges/the-report/problem) (often involves date comparisons, though not explicitly requiring date functions in this specific problem)
    * Many problems in the "Advanced Select" section might involve date manipulation.
* **Interview Questions:**
    1. What is the difference between `DATETIME` and `TIMESTAMP`?
    2. When would you use `DATE` instead of `DATETIME`?
    3. Explain how `TIMESTAMP` can be automatically updated in some RDBMS.
    4. How do you store only the year of a specific event?
    5. What are the advantages of using a dedicated date/time datatype over storing dates as strings?
    6. How can you extract only the month from a `DATETIME` column? (Mention functions, if applicable to the RDBMS)
    7. What is the default format for `DATE` and `DATETIME` in SQL?
    8. How does timezone handling differ between `DATETIME` and `TIMESTAMP`?
    9. Can you perform arithmetic operations on date and time types? Give an example.
    10. What issues might arise when migrating date and time data between different database systems?

### • Boolean Type

* **Subtopics:**
    * `BOOLEAN`/`BOOL`: Stores `TRUE` or `FALSE`
    * Representation: Often `1` for `TRUE` and `0` for `FALSE` (or `NULL`) in some databases
* **HackerRank Questions:** (Implicitly used in `WHERE` clauses)
    * Any problem involving conditions that evaluate to true/false.
* **Interview Questions:**
    1. Does SQL have a native `BOOLEAN` datatype? Explain. (Note: Varies by RDBMS, e.g., MySQL has `TINYINT(1)` which acts as boolean)
    2. How is `TRUE` and `FALSE` typically represented in databases that don't have a direct `BOOLEAN` type?
    3. When would you use a `BOOLEAN` type in your database schema?
    4. Can `BOOLEAN` columns be `NULL`? What does `NULL` signify in this context?
    5. Give an example of a query using a `BOOLEAN` column.
    6. What are the benefits of using a `BOOLEAN` type over an `INT` (0 or 1)?
    7. Are there any performance implications when using a `BOOLEAN` type?
    8. How do you insert `TRUE` or `FALSE` values into a `BOOLEAN` column?
    9. What is the size of a `BOOLEAN` column in memory?
    10. How would you handle a "tri-state" logic (true, false, unknown) if you only have a boolean type?

### • Choosing the Right Datatype

* **Subtopics:**
    * Storage efficiency
    * Data integrity
    * Performance of queries
    * Range and precision requirements
    * Future scalability
* **HackerRank Questions:** (Conceptual)
    * Understanding data types is fundamental for efficient query writing.
* **Interview Questions:**
    1. What factors should you consider when choosing a datatype for a column?
    2. Why is choosing the correct datatype important for database performance?
    3. How can an incorrect datatype choice lead to data integrity issues?
    4. If you're storing a country code (e.g., "US", "UK"), which string datatype would you choose and why?
    5. You need to store product prices that can go up to 99999.99. Which datatype is most appropriate?
    6. When designing a table, how do you decide if a numeric column should be signed or unsigned?
    7. Explain the concept of "data type mismatch" and its implications.
    8. How does choosing a smaller, more precise datatype benefit your database?
    9. What are the risks of using a generic, overly large datatype for all columns (e.g., `VARCHAR(255)` for everything)?
    10. How does the choice of datatype impact indexing strategies?

## 3. Constraints

### • Primary Key

* **Subtopics:**
    * Uniquely identifies each row in a table.
    * Cannot contain `NULL` values (NOT NULL).
    * Must be unique.
    * Automatically creates a unique index.
    * One primary key per table.
* **HackerRank Questions:** (Implicitly used in many problems, especially those involving `JOIN`s)
    * Problems requiring distinct rows or linking tables.
* **Interview Questions:**
    1. What is a Primary Key?
    2. What are the two main properties of a Primary Key?
    3. Can a table have more than one Primary Key? Explain.
    4. Can a Primary Key column contain `NULL` values? Why or why not?
    5. What is the purpose of a composite Primary Key? Give an example.
    6. How does a Primary Key help in maintaining data integrity?
    7. Does a Primary Key automatically create an index? What are the benefits of this?
    8. What happens if you try to insert a duplicate value into a Primary Key column?
    9. How do you define a Primary Key when creating a table?
    10. What is the difference between a Primary Key and a Unique Key?

### • Foreign Key

* **Subtopics:**
    * Establishes a link between two tables.
    * References the Primary Key of another table (or a Unique Key).
    * Ensures referential integrity.
    * `ON DELETE` and `ON UPDATE` actions (`CASCADE`, `SET NULL`, `RESTRICT`/`NO ACTION`)
* **HackerRank Questions:** (Crucial for `JOIN` problems)
    * [The Report](https://www.hackerrank.com/challenges/the-report/problem)
    * [Average Population of Each Continent](https://www.hackerrank.com/challenges/average-population-of-each-continent/problem)
    * [Ollivander's Inventory](https://www.hackerrank.com/challenges/ollivanders-inventory/problem)
    * Any problem involving relationships between tables.
* **Interview Questions:**
    1. What is a Foreign Key and its purpose?
    2. How does a Foreign Key relate to a Primary Key?
    3. Explain referential integrity in the context of Foreign Keys.
    4. What are the different `ON DELETE` actions for a Foreign Key? Describe each.
    5. When would you use `ON UPDATE CASCADE`?
    6. Can a Foreign Key column contain `NULL` values? When would this be allowed?
    7. What happens if you try to delete a row that is referenced by a Foreign Key with `RESTRICT` action?
    8. How do you define a Foreign Key when creating a table?
    9. What are the advantages of using Foreign Keys?
    10. Can a Foreign Key reference a column that is not a Primary Key? If so, what must that column be?

### • Unique

* **Subtopics:**
    * Ensures all values in a column are unique.
    * Allows `NULL` values (but only one `NULL` if permitted by the specific RDBMS).
    * Can have multiple `UNIQUE` constraints per table.
* **HackerRank Questions:** (Implicitly used when ensuring distinctness, e.g., `SELECT DISTINCT`)
    * Problems that require selecting unique identifiers.
* **Interview Questions:**
    1. What is a `UNIQUE` constraint?
    2. What is the main difference between a `UNIQUE` constraint and a `PRIMARY KEY`?
    3. Can a column with a `UNIQUE` constraint contain `NULL` values? How many?
    4. Give an example scenario where a `UNIQUE` constraint would be more appropriate than a `PRIMARY KEY`.
    5. Can you have multiple `UNIQUE` constraints on different columns in the same table?
    6. Does a `UNIQUE` constraint create an index?
    7. What happens if you try to insert a duplicate value into a column with a `UNIQUE` constraint?
    8. How do you define a `UNIQUE` constraint?
    9. What is a composite `UNIQUE` constraint?
    10. Are `UNIQUE` constraints always implicitly indexed?

### • Not Null

* **Subtopics:**
    * Ensures a column cannot have `NULL` values.
    * Every row must have a value for that column.
* **HackerRank Questions:** (Implicitly assumed in many problems where data presence is guaranteed)
    * Any problem where you expect data to always be present in a column.
* **Interview Questions:**
    1. What is the purpose of the `NOT NULL` constraint?
    2. Can a Primary Key column be `NULL`? Does it require a `NOT NULL` constraint explicitly?
    3. What happens if you try to insert a row without providing a value for a `NOT NULL` column?
    4. When would you use a `NOT NULL` constraint? Give an example.
    5. What is the difference between an empty string (`''`) and `NULL`?
    6. Can you add a `NOT NULL` constraint to an existing column that already contains `NULL` values? How would you handle this?
    7. What are the benefits of using `NOT NULL` constraints for data integrity?
    8. How does `NOT NULL` affect query performance?
    9. What is the default nullability of a column if not specified?
    10. Can a `FOREIGN KEY` column be `NOT NULL`?

### • Default

* **Subtopics:**
    * Specifies a default value for a column when no value is provided during insertion.
    * Ensures a value is always present, even if not explicitly given.
* **HackerRank Questions:** (Not directly tested, but good for understanding data insertion)
    * Any `INSERT` statement implicitly involves default values if not specified.
* **Interview Questions:**
    1. What is the purpose of the `DEFAULT` constraint?
    2. When is the `DEFAULT` value applied to a column?
    3. Can a `DEFAULT` value be a function (e.g., `CURRENT_TIMESTAMP`)? Give an example.
    4. If a column has both `NOT NULL` and `DEFAULT` constraints, what happens if no value is provided during insertion?
    5. Can you change the `DEFAULT` value of an existing column?
    6. What is the difference between `NULL` and a `DEFAULT` value?
    7. Provide a scenario where a `DEFAULT` constraint would be very useful.
    8. Does a `DEFAULT` constraint override an explicit value provided during `INSERT`?
    9. Are `DEFAULT` values stored directly in the table data or are they applied at the database engine level?
    10. What are the performance implications of using `DEFAULT` constraints?

### • Check

* **Subtopics:**
    * Defines a condition that each row must satisfy.
    * Ensures data falls within a specified range or meets certain criteria.
* **HackerRank Questions:** (Conceptual)
    * Not commonly tested directly, but good for understanding data validation.
* **Interview Questions:**
    1. What is a `CHECK` constraint used for?
    2. Give an example of a scenario where a `CHECK` constraint would be appropriate.
    3. Can a `CHECK` constraint refer to values in other columns of the same row?
    4. What happens if you try to insert or update a row that violates a `CHECK` constraint?
    5. Are `CHECK` constraints universally supported across all RDBMS?
    6. What is the difference between a `CHECK` constraint and a `WHERE` clause in a `SELECT` statement?
    7. Can you define a `CHECK` constraint that depends on the current date or time?
    8. What are the benefits of enforcing data validation at the database level using `CHECK` constraints?
    9. Are `CHECK` constraints considered as important for data integrity as Primary Keys or Foreign Keys? Why?
    10. How would you modify an existing `CHECK` constraint?

### • Auto Increment

* **Subtopics:**
    * Automatically generates unique sequential numbers for a column.
    * Often used for Primary Keys.
    * Also known as `IDENTITY` (SQL Server), `SERIAL` (PostgreSQL).
* **HackerRank Questions:** (Not directly tested, but common in table creation)
    * Any problem where an ID column is present and assumed to be unique.
* **Interview Questions:**
    1. What is the purpose of `AUTO_INCREMENT` (or `IDENTITY`/`SERIAL`)?
    2. Which datatype is typically used for `AUTO_INCREMENT` columns?
    3. Can an `AUTO_INCREMENT` column be part of a composite Primary Key?
    4. What happens to the `AUTO_INCREMENT` counter when you delete rows? (Varies by RDBMS)
    5. Can you explicitly insert a value into an `AUTO_INCREMENT` column?
    6. When would you reset the `AUTO_INCREMENT` counter? How would you do it?
    7. What are the advantages of using `AUTO_INCREMENT` for Primary Keys?
    8. Are `AUTO_INCREMENT` values guaranteed to be consecutive without gaps? Explain.
    9. What is the maximum value an `AUTO_INCREMENT` column can reach?
    10. How does `AUTO_INCREMENT` ensure uniqueness?

## 4. Overview of SQL Statements

### • DDL (CREATE, ALTER, DROP)

* **Subtopics:**
    * **CREATE:** Defines database objects (tables, views, indexes, databases, schemas).
        * `CREATE DATABASE`, `CREATE TABLE`, `CREATE INDEX`, `CREATE VIEW`
    * **ALTER:** Modifies the structure of existing database objects.
        * `ALTER TABLE ADD COLUMN`, `ALTER TABLE DROP COLUMN`, `ALTER TABLE MODIFY COLUMN`, `ALTER TABLE RENAME COLUMN`
    * **DROP:** Deletes database objects.
        * `DROP TABLE`, `DROP DATABASE`, `DROP INDEX`, `DROP VIEW`
* **HackerRank Questions:** (Conceptual, often provided schema, but understanding DDL helps)
    * None directly, as HackerRank typically provides the schema.
* **Interview Questions:**
    1. What does DDL stand for?
    2. List the main DDL commands.
    3. Explain the difference between `CREATE TABLE` and `ALTER TABLE`.
    4. What is the effect of `DROP TABLE`? Can it be reversed?
    5. How would you add a new column to an existing table?
    6. How would you rename a column in an existing table?
    7. What is the purpose of `CREATE INDEX`?
    8. When would you use `DROP DATABASE`?
    9. Can DDL statements be rolled back? Explain.
    10. What is a "schema" in the context of DDL?

### • DML (INSERT, UPDATE, DELETE)

* **Subtopics:**
    * **INSERT:** Adds new rows of data into a table.
        * `INSERT INTO table_name VALUES (...)`
        * `INSERT INTO table_name (column1, ...) VALUES (...)`
        * `INSERT INTO table_name SELECT ...` (insert from another query)
    * **UPDATE:** Modifies existing data in a table.
        * `UPDATE table_name SET column1 = value1 WHERE condition`
    * **DELETE:** Removes rows from a table.
        * `DELETE FROM table_name WHERE condition`
        * `DELETE FROM table_name` (deletes all rows)
* **HackerRank Questions:** (Fundamental for many problems)
    * Not directly provided for `INSERT`, `UPDATE`, `DELETE` operations, but you need to understand their effect on data for problem solving.
* **Interview Questions:**
    1. What does DML stand for?
    2. List the main DML commands.
    3. Explain the difference between `INSERT INTO` and `UPDATE`.
    4. How do you insert multiple rows at once using a single `INSERT` statement?
    5. What is the purpose of the `WHERE` clause in `UPDATE` and `DELETE` statements?
    6. What happens if you run `DELETE FROM table_name` without a `WHERE` clause?
    7. Can DML statements be rolled back?
    8. Give an example of an `UPDATE` statement.
    9. What is the difference between `DELETE` and `TRUNCATE`?
    10. How can you insert data into a table based on the result of a `SELECT` query?

### • DQL (SELECT)

* **Subtopics:**
    * **SELECT:** Retrieves data from one or more tables.
        * Basic `SELECT *`, `SELECT column_name`
        * `WHERE`, `GROUP BY`, `HAVING`, `ORDER BY`, `LIMIT` clauses
        * Aggregate functions, joins, subqueries
* **HackerRank Questions:** (The core of most HackerRank SQL problems)
    * All "Select" category problems.
    * All "Basic Join" problems.
    * All "Aggregation" problems.
    * All "Advanced Select" problems.
* **Interview Questions:**
    1. What does DQL stand for?
    2. What is the primary purpose of the `SELECT` statement?
    3. What is the difference between `SELECT *` and `SELECT column_name`?
    4. Explain the order of execution of clauses in a `SELECT` statement (e.g., `FROM`, `WHERE`, `GROUP BY`, `HAVING`, `SELECT`, `ORDER BY`).
    5. What is the role of the `FROM` clause?
    6. Can you retrieve data from multiple tables using `SELECT`? How?
    7. What is `SELECT DISTINCT` used for?
    8. How do you filter results in a `SELECT` query?
    9. Give an example of a simple `SELECT` statement.
    10. What are aliases in `SELECT` statements, and why are they used?

### • TCL (COMMIT, ROLLBACK, SAVEPOINT)

* **Subtopics:**
    * **COMMIT:** Makes all changes in the current transaction permanent.
    * **ROLLBACK:** Undoes all changes in the current transaction.
    * **SAVEPOINT:** Sets a point within a transaction to which you can roll back.
    * Transactions: A logical unit of work (ACID properties).
* **HackerRank Questions:** (Conceptual, not directly tested on HackerRank)
    * None directly.
* **Interview Questions:**
    1. What does TCL stand for?
    2. Explain the concept of a "transaction" in SQL.
    3. What are the ACID properties of a transaction? Describe each briefly.
    4. What is the purpose of `COMMIT`?
    5. When would you use `ROLLBACK`?
    6. Explain `SAVEPOINT` and its utility.
    7. Are DDL commands implicitly committed?
    8. What is the default transaction behavior in most RDBMS (e.g., auto-commit)?
    9. Give a scenario where using `SAVEPOINT` would be beneficial.
    10. What happens if a system crashes in the middle of a transaction before a `COMMIT`?

### • DCL (GRANT, REVOKE)

* **Subtopics:**
    * **GRANT:** Gives users specific permissions on database objects.
        * `GRANT SELECT ON table TO user`
        * `GRANT ALL PRIVILEGES ON database TO user`
    * **REVOKE:** Removes previously granted permissions.
        * `REVOKE DELETE ON table FROM user`
    * Roles and Privileges: Managing access control.
* **HackerRank Questions:** (Conceptual)
    * None directly.
* **Interview Questions:**
    1. What does DCL stand for?
    2. What is the purpose of `GRANT`?
    3. When would you use `REVOKE`?
    4. How do you grant a user permission to select data from a specific table?
    5. How do you remove a user's permission to insert data into a table?
    6. What is the difference between a "user" and a "role" in SQL?
    7. Why is access control important in a database system?
    8. What are some common privileges that can be granted or revoked?
    9. Can you grant permissions on an entire database? How?
    10. What are the security implications of poorly managed DCL?

## 5. Data Query Language (DQL)

### • SELECT Statement

* **Subtopics:**
    * Basic syntax: `SELECT columns FROM table`
    * Selecting all columns (`*`)
    * Selecting specific columns
    * Using aliases for columns (`AS`)
    * Performing simple calculations in `SELECT`
* **HackerRank Questions:**
    * [Revising the Select Query I](https://www.hackerrank.com/challenges/revising-the-select-query/problem)
    * [Revising the Select Query II](https://www.hackerrank.com/challenges/revising-the-select-query-2/problem)
    * [Select All](https://www.hackerrank.com/challenges/select-all-from-table/problem)
    * [Select By ID](https://www.hackerrank.com/challenges/select-by-id/problem)
    * [Japanese Cities' Attributes](https://www.hackerrank.com/challenges/japanese-cities-attributes/problem)
* **Interview Questions:**
    1. What is the fundamental purpose of the `SELECT` statement?
    2. When would you use `SELECT *` versus specifying individual columns?
    3. How do you rename a column in the output of a `SELECT` query?
    4. Can you perform arithmetic operations directly within a `SELECT` statement? Give an example.
    5. What is the role of the `FROM` clause in a `SELECT` statement?
    6. How do you select data from multiple tables using a simple `SELECT`? (Hint: Cross Join is implied here initially)
    7. Can you use a `SELECT` statement to query system tables?
    8. Explain the concept of projection in the context of `SELECT`.
    9. What are some best practices for writing readable `SELECT` statements?
    10. How do you handle `NULL` values when performing calculations in a `SELECT` statement?

### • SELECT DISTINCT

* **Subtopics:**
    * Removes duplicate rows from the result set.
    * Applies to all selected columns.
* **HackerRank Questions:**
    * [Weather Observation Station 3](https://www.hackerrank.com/challenges/weather-observation-station-3/problem)
    * [Weather Observation Station 4](https://www.hackerrank.com/challenges/weather-observation-station-4/problem)
    * [African Cities](https://www.hackerrank.com/challenges/african-cities/problem)
* **Interview Questions:**
    1. What is `SELECT DISTINCT` used for?
    2. How does `DISTINCT` work when applied to multiple columns?
    3. Does `DISTINCT` consider `NULL` values as duplicates?
    4. What is the difference between `GROUP BY` and `DISTINCT`? When would you use one over the other?
    5. Are there any performance implications when using `DISTINCT`?
    6. Can `DISTINCT` be used with aggregate functions?
    7. Give an example of a query where `DISTINCT` would be necessary.
    8. How would you count the number of unique values in a column?
    9. What happens if you use `DISTINCT` with `ORDER BY`?
    10. Is `DISTINCT` applied before or after `WHERE` and `GROUP BY`?

### • WHERE Clause

* **Subtopics:**
    * Filters rows based on a specified condition.
    * Evaluates to `TRUE`, `FALSE`, or `UNKNOWN` (for `NULL`).
    * Can use comparison, logical, and special operators.
* **HackerRank Questions:**
    * [Weather Observation Station 5](https://www.hackerrank.com/challenges/weather-observation-station-5/problem) (implicitly involves filtering logic)
    * [Employee Names](https://www.hackerrank.com/challenges/employee-names/problem)
    * [Higher Than 75 Marks](https://www.hackerrank.com/challenges/higher-than-75-marks/problem)
    * Numerous problems requiring specific row selection.
* **Interview Questions:**
    1. What is the purpose of the `WHERE` clause?
    2. Can you use aggregate functions directly in a `WHERE` clause? Why or why not?
    3. What is the order of execution of `WHERE` clause within a `SELECT` statement?
    4. How does `NULL` affect conditions in a `WHERE` clause?
    5. Give an example of a `WHERE` clause using a logical operator.
    6. What is the difference between `=`, `IS NULL`, and `IS NOT NULL`?
    7. Can you use arithmetic operations in a `WHERE` clause?
    8. How does `WHERE` clause improve query performance?
    9. What are some common mistakes when using the `WHERE` clause?
    10. Can you filter rows based on a subquery in the `WHERE` clause?

### • BETWEEN, IN, LIKE, IS NULL

* **Subtopics:**
    * **BETWEEN:** Tests if a value is within a range (inclusive).
        * `column BETWEEN value1 AND value2`
    * **IN:** Tests if a value matches any value in a list or subquery.
        * `column IN (value1, value2, ...)`
    * **LIKE:** Tests if a string matches a specified pattern.
        * Wildcard characters: `%` (any string), `_` (any single character)
        * `column LIKE 'pattern'`
    * **IS NULL / IS NOT NULL:** Tests for `NULL` values.
* **HackerRank Questions:**
    * [Weather Observation Station 6](https://www.hackerrank.com/challenges/weather-observation-station-6/problem) (LIKE)
    * [Weather Observation Station 11](https://www.hackerrank.com/challenges/weather-observation-station-11/problem) (LIKE, OR)
    * [Japanese Cities' Names](https://www.hackerrank.com/challenges/japanese-cities-names/problem) (WHERE clause)
    * Many problems involve filtering using these operators.
* **Interview Questions:**
    1. Explain the functionality of `BETWEEN`. Is the range inclusive or exclusive?
    2. When would you use `IN` instead of a series of `OR` conditions?
    3. What are the two main wildcard characters used with `LIKE`, and what do they represent?
    4. How do you find all names that start with 'A' using `LIKE`?
    5. Why can't you use `=` to check for `NULL` values? What is the correct way?
    6. Can `IN` be used with a subquery? Give an example.
    7. What is the equivalent of `NOT IN` using `EXISTS`?
    8. How does `LIKE` handle case sensitivity? (Note: Varies by RDBMS, often depends on collation)
    9. Give a scenario where `IS NOT NULL` would be essential.
    10. Can `BETWEEN` be used with date/time data types?

### • LIMIT, OFFSET

* **Subtopics:**
    * **LIMIT:** Restricts the number of rows returned by a query.
    * **OFFSET:** Specifies the starting point for retrieving rows after a certain number of rows have been skipped.
    * Used for pagination.
* **HackerRank Questions:**
    * [Weather Observation Station 5](https://www.hackerrank.com/challenges/weather-observation-station-5/problem) (Requires `LIMIT`)
    * [The Blunder](https://www.hackerrank.com/challenges/the-blunder/problem) (Requires `LIMIT`)
    * [Top Earners](https://www.hackerrank.com/challenges/top-earners/problem) (Requires `LIMIT`)
* **Interview Questions:**
    1. What is the purpose of `LIMIT` in a `SELECT` statement?
    2. How do `LIMIT` and `OFFSET` work together for pagination?
    3. Are `LIMIT` and `OFFSET` part of the ANSI SQL standard? (Note: `FETCH FIRST`/`OFFSET` are standard, `LIMIT` is MySQL/PostgreSQL specific).
    4. How do you select the second highest salary using `LIMIT` and `OFFSET`?
    5. What happens if you use `LIMIT` without `ORDER BY`?
    6. Can `LIMIT` be used with `INSERT` or `UPDATE` statements?
    7. What are the performance considerations when using large `OFFSET` values?
    8. How would you retrieve the first 10 records from a table?
    9. What is the alternative to `LIMIT`/`OFFSET` in SQL Server and Oracle?
    10. Explain a real-world scenario where `LIMIT` and `OFFSET` would be useful.

## 6. Operators

### • Arithmetic Operators: +, -, \*, /, %

* **Subtopics:**
    * Addition, Subtraction, Multiplication, Division, Modulo.
    * Used in `SELECT` lists and `WHERE` clauses.
* **HackerRank Questions:**
    * [The Blunder](https://www.hackerrank.com/challenges/the-blunder/problem) (involves arithmetic to remove zeros)
    * [Average Population](https://www.hackerrank.com/challenges/average-population/problem) (implicitly involves division)
    * Any problem involving calculations on numeric columns.
* **Interview Questions:**
    1. List the common arithmetic operators in SQL.
    2. How can you perform a calculation on two columns in a `SELECT` statement?
    3. What is the modulo operator (`%`) used for? Give an example.
    4. How does division by zero behave in SQL?
    5. Can arithmetic operators be used in a `WHERE` clause? Provide an example.
    6. What is operator precedence in SQL?
    7. How do `NULL` values affect arithmetic operations?
    8. Can you use arithmetic operators with date and time data types? (e.g., adding days)
    9. What is the difference between integer division and floating-point division in SQL?
    10. How would you round the result of an arithmetic operation?

### • Comparison Operators: =, !=, <>, <, >, <=, >=

* **Subtopics:**
    * Equal to (`=`)
    * Not equal to (`!=` or `<>`)
    * Less than (`<`)
    * Greater than (`>`)
    * Less than or equal to (`<=`)
    * Greater than or equal to (`>=`)
* **HackerRank Questions:**
    * [Higher Than 75 Marks](https://www.hackerrank.com/challenges/higher-than-75-marks/problem)
    * [Japanese Cities' Attributes](https://www.hackerrank.com/challenges/japanese-cities-attributes/problem)
    * Fundamental to all `WHERE` clause filtering.
* **Interview Questions:**
    1. List the common comparison operators in SQL.
    2. What is the difference between `!=` and `<>`?
    3. Can you compare strings using comparison operators? How does it work?
    4. How do comparison operators handle `NULL` values?
    5. Give an example of a `WHERE` clause using `>=`.
    6. What is the result of `10 = NULL`? Why?
    7. Can comparison operators be used with date/time data types?
    8. What is the order of evaluation for multiple comparison operators in a single condition?
    9. When would you use a comparison operator instead of `BETWEEN`?
    10. Explain how character sets and collations can impact string comparisons.

### • Logical Operators: AND, OR, NOT

* **Subtopics:**
    * **AND:** Returns `TRUE` if all conditions are `TRUE`.
    * **OR:** Returns `TRUE` if any condition is `TRUE`.
    * **NOT:** Negates a condition.
    * Operator precedence (NOT > AND > OR)
* **HackerRank Questions:**
    * [Weather Observation Station 11](https://www.hackerrank.com/challenges/weather-observation-station-11/problem) (AND, OR)
    * [Weather Observation Station 12](https://www.hackerrank.com/challenges/weather-observation-station-12/problem)
    * Many problems requiring complex filtering logic.
* **Interview Questions:**
    1. Explain the functionality of `AND`, `OR`, and `NOT` operators.
    2. What is the order of precedence for logical operators?
    3. How can you ensure a specific order of evaluation when using multiple logical operators?
    4. What is the result of `TRUE AND NULL`? What about `FALSE OR NULL`?
    5. Give an example of a query using `NOT` with `LIKE`.
    6. When would you use `OR` over `IN`?
    7. How do logical operators impact query performance?
    8. Can you combine logical operators with arithmetic and comparison operators?
    9. What is "short-circuiting" in the context of logical operators? (Though not always guaranteed in SQL)
    10. Describe a complex `WHERE` clause condition that uses all three logical operators.

### • Special Operators: IN, BETWEEN, LIKE, IS NULL

* **Subtopics:** (Reiterated for emphasis as operators)
    * `IN`
    * `BETWEEN`
    * `LIKE`
    * `IS NULL / IS NOT NULL`
    * `EXISTS` (often considered a special operator too)
* **HackerRank Questions:** (Already covered in DQL section, but good to link here)
    * [Weather Observation Station 6](https://www.hackerrank.com/challenges/weather-observation-station-6/problem)
    * [Weather Observation Station 11](https://www.hackerrank.com/challenges/weather-observation-station-11/problem)
* **Interview Questions:**
    1. Beyond the common comparison operators, what are some "special" operators in SQL?
    2. How is `IN` different from a simple list of `OR` conditions in terms of performance or readability?
    3. When using `LIKE` with wildcards, how do you search for the literal wildcard characters themselves (e.g., `_` or `%`)?
    4. Explain the difference between `IS NULL` and an empty string comparison.
    5. What is the `NOT BETWEEN` operator used for?
    6. Can `BETWEEN` be used with text columns? How does it sort?
    7. What is the purpose of the `EXISTS` operator? (Introduced here as it often falls into "special" category)
    8. Can you combine special operators with logical operators? Give an example.
    9. What are the advantages of using these special operators over equivalent, more verbose conditions?
    10. Are there any performance considerations unique to `LIKE` with leading wildcards (e.g., `%value`)?

## 7. Functions

### • Aggregate Functions: COUNT(), SUM(), AVG(), MIN(), MAX()

* **Subtopics:**
    * Operate on a set of rows and return a single summary value.
    * Often used with `GROUP BY`.
    * `COUNT(*)` vs `COUNT(column_name)` vs `COUNT(DISTINCT column_name)`
    * Handling `NULL` values.
* **HackerRank Questions:**
    * [Revising Aggregations - The Count Function](https://www.hackerrank.com/challenges/revising-aggregations-the-count-function/problem)
    * [Revising Aggregations - Sum Function](https://www.hackerrank.com/challenges/revising-aggregations-sum-function/problem)
    * [Revising Aggregations - Averages](https://www.hackerrank.com/challenges/revising-aggregations-averages/problem)
    * [Population Density Difference](https://www.hackerrank.com/challenges/population-density-difference/problem)
    * [The Sum Function](https://www.hackerrank.com/challenges/the-sum-function/problem)
    * [Average Population](https://www.hackerrank.com/challenges/average-population/problem)
    * [Japan Population](https://www.hackerrank.com/challenges/japan-population/problem)
    * [Population Census](https://www.hackerrank.com/challenges/population-census/problem)
    * [Top Earners](https://www.hackerrank.com/challenges/top-earners/problem) (MAX, COUNT)
* **Interview Questions:**
    1. What is an aggregate function in SQL?
    2. Explain the difference between `COUNT(*)` and `COUNT(column_name)`.
    3. How does `COUNT(DISTINCT column_name)` work?
    4. How do `SUM()`, `AVG()`, `MIN()`, and `MAX()` handle `NULL` values?
    5. Can you use aggregate functions in a `WHERE` clause? Why or why not?
    6. When would you use `AVG()` instead of calculating the average manually?
    7. What is the output of `MIN()` and `MAX()` on string data?
    8. Can you combine multiple aggregate functions in a single `SELECT` statement?
    9. Explain the concept of "grouping" in relation to aggregate functions.
    10. What are some performance considerations when using aggregate functions on large datasets?

### • String Functions: CONCAT(), LENGTH(), LOWER(), UPPER()

* **Subtopics:**
    * `CONCAT(string1, string2, ...)`: Joins strings.
    * `LENGTH(string)`: Returns the length of a string. (`LEN` in SQL Server, `LENGTH` or `CHAR_LENGTH` in others)
    * `LOWER(string)`: Converts string to lowercase.
    * `UPPER(string)`: Converts string to uppercase.
    * `SUBSTRING(string, start, length)`: Extracts a substring.
    * `TRIM(string)`: Removes leading/trailing spaces.
    * `REPLACE(string, old_substring, new_substring)`: Replaces occurrences of a substring.
* **HackerRank Questions:**
    * [Higher Than 75 Marks](https://www.hackerrank.com/challenges/higher-than-75-marks/problem) (SUBSTRING or RIGHT)
    * [The Blunder](https://www.hackerrank.com/challenges/the-blunder/problem) (REPLACE)
    * [Weather Observation Station 12](https://www.hackerrank.com/challenges/weather-observation-station-12/problem) (LOWER, UPPER, SUBSTRING)
* **Interview Questions:**
    1. Name three common string functions and explain their purpose.
    2. How do you combine two columns into a single output column using a string function?
    3. What is the difference between `LENGTH()` and `CHAR_LENGTH()` (if applicable to RDBMS)?
    4. How would you convert a column's values to all uppercase for comparison purposes?
    5. Explain how `SUBSTRING()` works with an example.
    6. What is `TRIM()` used for? Why is it important?
    7. How do you replace specific characters within a string in SQL?
    8. What are the performance implications of using string functions on large text columns?
    9. Can string functions be used in `WHERE` clauses? Give an example.
    10. How do different character encodings affect string function behavior?

### • Date Functions: NOW(), CURDATE(), DATEDIFF()

* **Subtopics:**
    * `NOW()`/`GETDATE()`: Returns current date and time.
    * `CURDATE()`/`CURRENT_DATE`: Returns current date.
    * `CURTIME()`/`CURRENT_TIME`: Returns current time.
    * `DATEDIFF(unit, date1, date2)`: Calculates difference between dates.
    * `DATE_ADD()`/`DATE_SUB()`: Adds/subtracts intervals from dates.
    * `YEAR()`, `MONTH()`, `DAY()`: Extracts parts of a date.
* **HackerRank Questions:**
    * [New Companies](https://www.hackerrank.com/challenges/new-companies/problem) (Often involves date logic, though not directly tested with these functions)
    * Problems might involve calculating age or time elapsed.
* **Interview Questions:**
    1. Name three common date functions and explain their use.
    2. What is the difference between `NOW()` and `CURDATE()`?
    3. How do you calculate the number of days between two dates?
    4. How would you add 5 days to a specific date in SQL?
    5. Can you extract only the year from a `DATETIME` column? How?
    6. What is the default date format returned by date functions?
    7. How do date functions handle timezones?
    8. Give an example of using a date function in a `WHERE` clause.
    9. What are the performance considerations when using date functions for filtering?
    10. How would you format a date to a specific string format (e.g., 'YYYY-MM-DD')?

### • Numeric Functions: ROUND(), CEIL(), FLOOR(), ABS()

* **Subtopics:**
    * `ROUND(number, decimals)`: Rounds a number to a specified number of decimal places.
    * `CEIL(number)`: Returns the smallest integer greater than or equal to the number (ceil).
    * `FLOOR(number)`: Returns the largest integer less than or equal to the number (floor).
    * `ABS(number)`: Returns the absolute value of a number.
    * `MOD(number, divisor)`: Returns the remainder of a division.
    * `POWER(base, exponent)`: Returns the base raised to the exponent.
* **HackerRank Questions:**
    * [The Blunder](https://www.hackerrank.com/challenges/the-blunder/problem) (implicitly involves rounding/casting to integer)
    * [Average Population](https://www.hackerrank.com/challenges/average-population/problem) (rounding averages)
* **Interview Questions:**
    1. Explain the difference between `CEIL()` and `FLOOR()`.
    2. What is `ROUND()` used for? How does it handle rounding .5?
    3. When would you use `ABS()`? Give an example.
    4. How do numeric functions handle `NULL` input?
    5. Can you use numeric functions in `GROUP BY` or `ORDER BY` clauses?
    6. What is the purpose of the `MOD()` function?
    7. How would you calculate the square root of a number in SQL? (Might need specific function like `SQRT()`)
    8. Are there any performance implications when using numeric functions?
    9. Can numeric functions be chained (e.g., `ROUND(AVG(...))`)?
    10. How do different database systems handle floating-point precision issues with numeric functions?

## 8. Grouping

### • GROUP BY Clause

* **Subtopics:**
    * Groups rows that have the same values in specified columns into summary rows.
    * Often used with aggregate functions.
    * All non-aggregated columns in `SELECT` must be in `GROUP BY`.
* **HackerRank Questions:**
    * [Average Population of Each Continent](https://www.hackerrank.com/challenges/average-population-of-each-continent/problem)
    * [Population Census](https://www.hackerrank.com/challenges/population-census/problem)
    * [Weather Observation Station 9](https://www.hackerrank.com/challenges/weather-observation-station-9/problem)
    * Any problem requiring aggregation per category.
* **Interview Questions:**
    1. What is the purpose of the `GROUP BY` clause?
    2. When is `GROUP BY` used in conjunction with aggregate functions?
    3. What is the rule regarding columns in the `SELECT` list when using `GROUP BY`?
    4. Can you group by multiple columns? Give an example.
    5. What is the logical order of execution for `GROUP BY` within a `SELECT` statement?
    6. How does `GROUP BY` handle `NULL` values in the grouping columns?
    7. Explain the concept of "grouping sets" or `ROLLUP`/`CUBE` (if aware).
    8. What are the performance implications of grouping on large datasets?
    9. Can you use aliases defined in the `SELECT` clause in the `GROUP BY` clause?
    10. How would you find the total sales for each product category?

### • HAVING Clause

* **Subtopics:**
    * Filters groups based on a specified condition.
    * Used after `GROUP BY`.
    * Can use aggregate functions in its condition.
* **HackerRank Questions:**
    * [The Report](https://www.hackerrank.com/challenges/the-report/problem) (implicitly involves filtering on aggregates)
    * [Ollivander's Inventory](https://www.hackerrank.com/challenges/ollivanders-inventory/problem) (complex joins and HAVING)
    * Any problem requiring filtering aggregated results.
* **Interview Questions:**
    1. What is the purpose of the `HAVING` clause?
    2. What is the main difference between `WHERE` and `HAVING`?
    3. When is `HAVING` clause evaluated in the `SELECT` statement's execution order?
    4. Can you use non-aggregated columns in a `HAVING` clause?
    5. Give an example of a query where `HAVING` would be essential.
    6. Can `HAVING` be used without `GROUP BY`? What happens then?
    7. How do `NULL` values affect `HAVING` conditions?
    8. What are the performance implications of using `HAVING` on large datasets?
    9. Can you use a subquery in a `HAVING` clause?
    10. How would you find departments where the average salary is greater than $50,000?

### • GROUP BY with Aggregates

* **Subtopics:**
    * Combining `GROUP BY` with `COUNT()`, `SUM()`, `AVG()`, `MIN()`, `MAX()`.
    * Understanding how aggregates operate on each group.
* **HackerRank Questions:**
    * [African Cities](https://www.hackerrank.com/challenges/african-cities/problem) (JOIN and GROUP BY)
    * [Contest Leaderboard](https://www.hackerrank.com/challenges/contest-leaderboard/problem) (Complex GROUP BY, ORDER BY, aggregate functions)
    * [The PADS](https://www.hackerrank.com/challenges/the-pads/problem) (GROUP BY, string manipulation)
* **Interview Questions:**
    1. How do `GROUP BY` and aggregate functions work together?
    2. Give an example of calculating the total quantity sold for each product.
    3. How would you find the number of employees in each department?
    4. Can you find the maximum salary within each job role?
    5. What happens if you use an aggregate function without a `GROUP BY` clause?
    6. Explain the concept of "grouping sets" or `ROLLUP`/`CUBE` (if aware).
    7. How would you identify product categories that have more than 10 products?
    8. What is the importance of aliases when using aggregates with `GROUP BY`?
    9. Can you apply `ORDER BY` on an aggregated result?
    10. Describe a scenario where you would need to use `GROUP BY` with both `SUM()` and `AVG()` in the same query.

### • Difference Between WHERE and HAVING

* **Subtopics:**
    * `WHERE` filters individual rows *before* grouping.
    * `HAVING` filters groups *after* grouping and aggregation.
    * `WHERE` cannot use aggregate functions directly.
    * `HAVING` can use aggregate functions.
* **HackerRank Questions:** (Implicitly tested when solving problems that require both row and group filtering)
* **Interview Questions:**
    1. What is the fundamental difference between `WHERE` and `HAVING`?
    2. Can you use `WHERE` and `HAVING` in the same query? If so, what is their order of execution?
    3. When should you use `WHERE` versus `HAVING` to filter results?
    4. Provide an example where using `WHERE` would be incorrect, and `HAVING` would be correct.
    5. Can you give an example where a condition could be placed in either `WHERE` or `HAVING`? What's the best practice?
    6. Which clause is processed first by the database engine, `WHERE` or `HAVING`?
    7. How does the performance differ between filtering with `WHERE` versus `HAVING`?
    8. Can you use non-aggregated columns in a `HAVING` clause if they are also in the `GROUP BY` clause?
    9. What happens if you try to use an aggregate function in a `WHERE` clause?
    10. Explain the concept of "pre-filtering" vs. "post-filtering" in relation to `WHERE` and `HAVING`.

## 9. Sorting

### • ORDER BY Clause

* **Subtopics:**
    * Sorts the result set of a query.
    * Can sort by one or more columns.
    * Default sort order is `ASC` (ascending).
* **HackerRank Questions:**
    * [Higher Than 75 Marks](https://www.hackerrank.com/challenges/higher-than-75-marks/problem)
    * [Employee Salaries](https://www.hackerrank.com/challenges/employee-salaries/problem)
    * [Type of Triangle](https://www.hackerrank.com/challenges/type-of-triangle/problem) (ORDER BY with complex logic)
    * Many problems require ordered output.
* **Interview Questions:**
    1. What is the purpose of the `ORDER BY` clause?
    2. What is the default sorting order if not specified?
    3. Can you sort by a column that is not selected in the `SELECT` list? (Varies by RDBMS, generally yes if it's from `FROM` clause)
    4. What is the logical order of execution for `ORDER BY` within a `SELECT` statement?
    5. How does `ORDER BY` handle `NULL` values? (Varies by RDBMS, usually puts them at the beginning or end).
    6. Can you use aliases defined in the `SELECT` clause in the `ORDER BY` clause?
    7. What are the performance implications of sorting large datasets?
    8. How would you sort data based on the length of a string column?
    9. Can `ORDER BY` be used with aggregate functions in the `SELECT` list?
    10. Describe a scenario where you would need to use `ORDER BY` on an expression rather than a simple column.

### • ASC vs DESC

* **Subtopics:**
    * `ASC`: Ascending order (A-Z, 0-9).
    * `DESC`: Descending order (Z-A, 9-0).
* **HackerRank Questions:**
    * [Top Earners](https://www.hackerrank.com/challenges/top-earners/problem)
    * [Weather Observation Station 5](https://www.hackerrank.com/challenges/weather-observation-station-5/problem)
    * Most sorting problems involve `ASC` or `DESC`.
* **Interview Questions:**
    1. What is the difference between `ASC` and `DESC`?
    2. How do you sort results in descending order?
    3. Can you specify `ASC` or `DESC` for individual columns when sorting by multiple columns?
    4. If you omit `ASC` or `DESC`, what is the default behavior?
    5. How do these keywords affect the sorting of text data?
    6. Can you sort by both `ASC` and `DESC` in the same `ORDER BY` clause? Give an example.
    7. What are the implications of sorting on character sets that have different collation rules?
    8. When would sorting in descending order be more useful?
    9. Does `ASC` or `DESC` influence the processing order of other clauses like `WHERE` or `GROUP BY`?
    10. How would you sort names alphabetically, but put 'Z' names first?

### • Sorting by Multiple Columns

* **Subtopics:**
    * Specifying multiple columns in `ORDER BY` clause.
    * Order of columns matters for tie-breaking.
    * Each column can have its own `ASC` or `DESC`.
* **HackerRank Questions:**
    * [Occupations](https://www.hackerrank.com/challenges/occupations/problem) (Complex sorting)
    * [Ollivander's Inventory](https://www.hackerrank.com/challenges/ollivanders-inventory/problem) (Multiple sorting criteria)
* **Interview Questions:**
    1. How do you sort a result set by multiple columns?
    2. Explain the significance of the order of columns in `ORDER BY`.
    3. Give an example of sorting by department name in ascending order, and then by employee salary in descending order within each department.
    4. What happens if two rows have the same value for the first sorting column?
    5. Can you mix `ASC` and `DESC` when sorting by multiple columns?
    6. What is the maximum number of columns you can sort by? (Theoretical, practically limited by performance).
    7. How does sorting by multiple columns impact query performance?
    8. Can you sort by a calculated expression that involves multiple columns?
    9. If you sort by three columns, and the first two are identical, which column determines the final order?
    10. Describe a business scenario where sorting by multiple criteria is essential.

## 10. Subquery

### • What is a Subquery?

* **Subtopics:**
    * A query nested inside another SQL query.
    * Also known as an inner query or inner select.
    * The inner query executes first, and its result is used by the outer query.
    * Can return a single value, a single row, a single column, or a table.
* **HackerRank Questions:** (Many HackerRank problems can be solved with subqueries)
    * [The Report](https://www.hackerrank.com/challenges/the-report/problem)
    * [Top Earners](https://www.hackerrank.com/challenges/top-earners/problem) (can be solved with subquery or LIMIT)
    * [Symmetric Pairs](https://www.hackerrank.com/challenges/symmetric-pairs/problem) (often involves subqueries)
* **Interview Questions:**
    1. What is a subquery?
    2. Why are subqueries used in SQL?
    3. What is the execution order between an outer query and an inner query?
    4. What are the different types of results a subquery can return?
    5. What are the advantages of using subqueries?
    6. Are there any disadvantages to using subqueries?
    7. Can a subquery have its own `WHERE`, `GROUP BY`, or `ORDER BY` clause?
    8. What is the difference between a subquery and a join (in terms of when to use them)?
    9. Can you write a subquery that references a column from the outer query?
    10. What is a common pitfall when using subqueries?

### • Types of Subqueries:

* **Scalar Subquery**
    * **Subtopics:**
        * Returns a single value (one row, one column).
        * Can be used in `SELECT` clause, `WHERE` clause, or `HAVING` clause.
    * **HackerRank Questions:** Any problem requiring a single aggregate value from a different context.
    * **Interview Questions:**
        1. What is a scalar subquery?
        2. Where can a scalar subquery be used in an outer query?
        3. Give an example of a scalar subquery used in a `SELECT` clause.
        4. What happens if a scalar subquery returns more than one row?
        5. Can a scalar subquery return `NULL`? How does it affect the outer query?
        6. When would you use a scalar subquery over a join?
        7. Explain a scenario where a scalar subquery is particularly useful.
        8. What are the performance considerations for scalar subqueries?
        9. Can a scalar subquery contain an aggregate function?
        10. How would you find the product with the highest price using a scalar subquery?

* **Row Subquery**
    * **Subtopics:**
        * Returns a single row (one or more columns).
        * Used in `WHERE` or `HAVING` clauses for row comparisons.
        * Often used with `IN`, `EXISTS`, or comparison operators.
    * **HackerRank Questions:** Problems like "Students who scored higher than the average in a subject."
    * **Interview Questions:**
        1. What is a row subquery?
        2. Where are row subqueries typically used?
        3. Give an example of a row subquery used with the `IN` operator.
        4. What happens if a row subquery returns multiple rows?
        5. How is a row subquery different from a scalar subquery?
        6. Can a row subquery be correlated?
        7. Provide a scenario where a row subquery is a good solution.
        8. What are the limitations of row subqueries?
        9. How do you compare multiple columns from the outer query to a row returned by a subquery?
        10. Can a row subquery return no rows? How does that affect the outer query?

* **Table Subquery**
    * **Subtopics:**
        * Returns a table (multiple rows, multiple columns).
        * Used in the `FROM` clause (derived table/inline view).
        * Used with `IN` or `EXISTS` for set comparisons.
    * **HackerRank Questions:**
        * [The Report](https://www.hackerrank.com/challenges/the-report/problem) (can be solved with a derived table)
        * [Occupations](https://www.hackerrank.com/challenges/occupations/problem) (can involve pivoting with derived tables)
    * **Interview Questions:**
        1. What is a table subquery (or derived table)?
        2. Where can a table subquery be used in an outer query?
        3. Give an example of a table subquery used in the `FROM` clause.
        4. What is the purpose of aliasing a table subquery?
        5. How does a table subquery differ from a regular view?
        6. Can a table subquery be correlated?
        7. When would you use a table subquery instead of a `JOIN`?
        8. What are the performance implications of using complex table subqueries?
        9. Can a table subquery have `GROUP BY` or `ORDER BY` clauses?
        10. How would you find the top N products by sales using a table subquery?

### • Subqueries in WHERE, FROM, and SELECT Clauses

* **Subtopics:**
    * **`WHERE` clause:** Most common, used for filtering.
    * **`FROM` clause:** Creates a temporary, derived table for the outer query.
    * **`SELECT` clause:** Scalar subquery, returns a single value for each row.
* **HackerRank Questions:** (Covers nearly all advanced HackerRank SQL problems)
    * Any problem requiring data from one context to filter or process data in another.
* **Interview Questions:**
    1. Explain the different places where a subquery can be used in a SQL statement.
    2. Provide an example of a subquery used in the `WHERE` clause.
    3. Provide an example of a subquery used in the `FROM` clause.
    4. Provide an example of a subquery used in the `SELECT` clause.
    5. What are the advantages of using a subquery in the `FROM` clause compared to a `JOIN`?
    6. When would you avoid using a subquery in the `SELECT` clause for performance reasons?
    7. Can a subquery in the `SELECT` clause access columns from the outer query?
    8. How does the RDBMS optimizer handle subqueries in different clauses?
    9. What is the benefit of using subqueries for modularity and readability?
    10. Describe a scenario where a single SQL statement needs subqueries in all three clauses (`SELECT`, `FROM`, `WHERE`).

## 11. Joins

### • INNER JOIN

* **Subtopics:**
    * Returns only the rows that have matching values in both tables.
    * The most common type of join.
    * Syntax: `FROM table1 INNER JOIN table2 ON condition`
* **HackerRank Questions:**
    * [Average Population of Each Continent](https://www.hackerrank.com/challenges/average-population-of-each-continent/problem)
    * [African Cities](https://www.hackerrank.com/challenges/african-cities/problem)
    * [The Report](https://www.hackerrank.com/challenges/the-report/problem)
    * [Ollivander's Inventory](https://www.hackerrank.com/challenges/ollivanders-inventory/problem)
    * Numerous problems requiring data from related tables.
* **Interview Questions:**
    1. What is an `INNER JOIN` used for?
    2. How does an `INNER JOIN` work?
    3. When would you use an `INNER JOIN`? Give a practical example.
    4. What happens if there are no matching values in the joined tables?
    5. Can you join more than two tables using `INNER JOIN`?
    6. What is the difference between `INNER JOIN` and a comma-separated list of tables in the `FROM` clause (implicit join)?
    7. How does the `ON` clause work with `INNER JOIN`?
    8. What are the performance considerations of `INNER JOIN`?
    9. Can an `INNER JOIN` produce a Cartesian product? When?
    10. How would you join an `Orders` table with a `Customers` table to retrieve orders with customer names?

### • LEFT JOIN

* **Subtopics:**
    * Returns all rows from the left table, and the matching rows from the right table.
    * If no match in the right table, `NULL` values are returned for right table columns.
    * Also known as `LEFT OUTER JOIN`.
* **HackerRank Questions:** (Problems where you need to see all records from one table, even if there's no match in another.)
* **Interview Questions:**
    1. What is a `LEFT JOIN` used for?
    2. How does a `LEFT JOIN` differ from an `INNER JOIN`?
    3. When would you use a `LEFT JOIN`? Give a practical example.
    4. What values appear in the right table's columns if there's no match?
    5. How would you find customers who have not placed any orders?
    6. Is `LEFT JOIN` the same as `LEFT OUTER JOIN`?
    7. Can you chain multiple `LEFT JOIN`s?
    8. What are the performance considerations of `LEFT JOIN`?
    9. How can you combine `LEFT JOIN` with `WHERE` to find unmatched rows?
    10. How would you list all employees and their respective department names, even if some employees are not assigned to any department?

### • RIGHT JOIN

* **Subtopics:**
    * Returns all rows from the right table, and the matching rows from the left table.
    * If no match in the left table, `NULL` values are returned for left table columns.
    * Also known as `RIGHT OUTER JOIN`.
* **HackerRank Questions:** (Similar to LEFT JOIN, just reversed)
* **Interview Questions:**
    1. What is a `RIGHT JOIN` used for?
    2. How does a `RIGHT JOIN` differ from a `LEFT JOIN`?
    3. When would you use a `RIGHT JOIN`? Give a practical example.
    4. What values appear in the left table's columns if there's no match?
    5. How would you find departments that have no employees?
    6. Is `RIGHT JOIN` the same as `RIGHT OUTER JOIN`?
    7. Can you always rewrite a `RIGHT JOIN` as a `LEFT JOIN`? How?
    8. What are the performance considerations of `RIGHT JOIN`?
    9. When is `RIGHT JOIN` generally less common than `LEFT JOIN`?
    10. How would you list all departments and their respective employee names, even if some departments have no employees?
### • FULL OUTER JOIN (if supported)

* **Subtopics:**
    * Returns all rows when there is a match in either the left or right table.
    * Returns `NULL` for columns from the table that doesn't have a match.
    * Combines the results of `LEFT JOIN` and `RIGHT JOIN`.
    * Not supported in MySQL directly (simulated with `UNION ALL`).
* **HackerRank Questions:** (Less common, but can be simulated if needed)
* **Interview Questions:**
    1. What is a `FULL OUTER JOIN` used for?
    2. How does `FULL OUTER JOIN` combine data from two tables?
    3. When would you use a `FULL OUTER JOIN`? Give a practical example.
    4. What values are returned for unmatched rows in both tables?
    5. Is `FULL OUTER JOIN` supported by all major RDBMS? Which ones don't?
    6. How can you simulate a `FULL OUTER JOIN` in a database that doesn't support it directly?
    7. What are the performance implications of `FULL OUTER JOIN`?
    8. Describe a scenario where you need to see all entries from two related but not perfectly overlapping lists.
    9. Can you combine `FULL OUTER JOIN` with `WHERE` to find records that exist in only one of the tables?
    10. What is the difference between a `FULL OUTER JOIN` and a `UNION` of `LEFT JOIN` and `RIGHT JOIN`?

### • CROSS JOIN

* **Subtopics:**
    * Returns the Cartesian product of the two tables.
    * Combines every row from the first table with every row from the second table.
    * No `ON` clause is used.
* **HackerRank Questions:** (Rarely explicitly used for solutions, but fundamental for understanding joins)
* **Interview Questions:**
    1. What is a `CROSS JOIN`?
    2. When would you typically use a `CROSS JOIN`?
    3. What is the result of a `CROSS JOIN` between a table with `M` rows and a table with `N` rows?
    4. Does a `CROSS JOIN` require an `ON` clause? Why or why not?
    5. What are the potential dangers or performance implications of using a `CROSS JOIN`?
    6. Can `CROSS JOIN` be used implicitly? How?
    7. Give a scenario where a `CROSS JOIN` could be useful (e.g., generating permutations, calendar dates).
    8. What is the difference between `CROSS JOIN` and `INNER JOIN` with a constantly true `ON` clause?
    9. How can `CROSS JOIN` be used to generate test data?
    10. Can you combine `CROSS JOIN` with `WHERE` to filter results?

### • Self Join

* **Subtopics:**
    * Joining a table to itself.
    * Requires table aliases to differentiate the two "copies" of the table.
    * Useful for hierarchical data or comparing rows within the same table.
* **HackerRank Questions:**
    * [The Report](https://www.hackerrank.com/challenges/the-report/problem) (can be solved with self-join logic)
    * [Students Marks](https://www.hackerrank.com/challenges/students-marks/problem) (Can be useful for comparing student scores to themselves)
* **Interview Questions:**
    1. What is a `SELF JOIN`?
    2. When would you use a `SELF JOIN`? Give a practical example.
    3. Why are table aliases mandatory for a `SELF JOIN`?
    4. How would you find employees who earn more than their direct managers?
    5. Can `SELF JOIN` be an `INNER JOIN`, `LEFT JOIN`, etc.?
    6. What are the performance considerations for `SELF JOIN`s, especially on large tables?
    7. Describe a scenario where you need to find pairs of users who share a common interest from a single table of user interests.
    8. How would you find all direct and indirect subordinates of an employee using `SELF JOIN` (if possible, with recursive CTEs for multiple levels)?
    9. What is the difference between a `SELF JOIN` and a regular join with two different tables?
    10. How would you find duplicate entries in a single table using a `SELF JOIN`?

### • USING vs ON Clause

* **Subtopics:**
    * **ON Clause:** Specifies a join condition using any valid comparison. More flexible.
        * `ON table1.column = table2.column`
    * **USING Clause:** Shorthand for `ON` when columns in both tables have the same name.
        * `USING (common_column_name)`
* **HackerRank Questions:** (Many HackerRank solutions use `ON`)
* **Interview Questions:**
    1. What is the purpose of the `ON` clause in a `JOIN`?
    2. When would you use the `USING` clause instead of `ON`?
    3. What is the main limitation of the `USING` clause?
    4. Can you use the `ON` clause for conditions other than equality? Give an example.
    5. Which clause (`ON` or `USING`) is more flexible? Why?
    6. Is there a performance difference between `ON` and `USING`?
    7. How do the results from `ON` and `USING` differ if multiple columns have the same name in both tables but are not all part of the join condition?
    8. Which clause is generally preferred for clarity and robustness in complex joins?
    9. Can `USING` be used with `FULL OUTER JOIN`?
    10. Provide an example where `USING` would simplify your join statement.

## 12. Co-Related Subquery

### • What is a Co-related Subquery?

* **Subtopics:**
    * An inner query that depends on the outer query for its execution.
    * The inner query executes once for each row processed by the outer query.
    * Often uses columns from the outer query in its `WHERE` clause.
* **HackerRank Questions:** (Many complex filtering problems can be solved with correlated subqueries)
    * [The Report](https://www.hackerrank.com/challenges/the-report/problem) (can be solved with correlated subqueries)
    * [Symmetric Pairs](https://www.hackerrank.com/challenges/symmetric-pairs/problem)
    * Finding records that are "top N" within a group.
* **Interview Questions:**
    1. What is a correlated subquery?
    2. How does a correlated subquery differ from a non-correlated subquery?
    3. Explain the execution flow of a correlated subquery.
    4. When would you use a correlated subquery? Give a practical example.
    5. Can correlated subqueries use aggregate functions?
    6. How does the `EXISTS` operator often work with correlated subqueries?
    7. What is the "linking" mechanism between the inner and outer queries in a correlated subquery?
    8. Provide an example of a correlated subquery that finds employees earning more than the average salary in their own department.
    9. Are correlated subqueries always slower than equivalent joins?
    10. What are the common performance issues associated with correlated subqueries?

### • Difference Between Normal and Co-related Subqueries

* **Subtopics:**
    * **Normal (Non-correlated):** Executes independently once, then outer query uses its result.
    * **Correlated:** Executes repeatedly, once for each candidate row of the outer query.
    * Dependency: Normal is independent, Correlated is dependent.
* **HackerRank Questions:** (Conceptual understanding is key to choosing the right approach)
* **Interview Questions:**
    1. Summarize the key differences between a normal (non-correlated) subquery and a correlated subquery.
    2. Which type of subquery executes first: normal or correlated?
    3. Can a normal subquery reference columns from the outer query? Why or why not?
    4. Which type of subquery is generally more performant for simple filtering?
    5. When would a normal subquery be preferred? When would a correlated subquery be preferred?
    6. Can a correlated subquery be rewritten as a join? Is it always better to do so?
    7. Give an example of a query that *must* use a correlated subquery because a normal subquery or join won't work.
    8. How does the database optimizer distinguish between the two types of subqueries?
    9. What are the "gotchas" or common errors when writing correlated subqueries?
    10. Explain the concept of "data flow" for both types of subqueries.

### • Performance Considerations

* **Subtopics:**
    * Correlated subqueries can be performance intensive due to repeated execution.
    * Indexes on linking columns are crucial.
    * Often can be rewritten as joins for better performance.
    * Sometimes, correlated subqueries are the most intuitive or only way.
* **HackerRank Questions:** (Implicit, as efficient solutions are often rewarded)
* **Interview Questions:**
    1. Why are correlated subqueries sometimes considered a performance bottleneck?
    2. What steps can you take to optimize a query that uses a correlated subquery?
    3. How do indexes help improve the performance of correlated subqueries?
    4. Is it always true that rewriting a correlated subquery as a join will result in better performance? Explain.
    5. When might a correlated subquery actually perform better than a complex join?
    6. What is the role of the database optimizer when encountering correlated subqueries?
    7. What impact does the size of the outer table have on the performance of a correlated subquery?
    8. How can `EXISTS` and `NOT EXISTS` improve performance with correlated subqueries compared to `IN` and `NOT IN`?
    9. Describe a scenario where a correlated subquery might be unavoidable or the most straightforward approach, despite potential performance concerns.
    10. What tools or techniques would you use to diagnose performance issues with correlated subqueries?

## 13. Data Definition Language (DDL)

### • CREATE TABLE

* **Subtopics:**
    * Syntax for defining table name, column names, data types, and constraints.
    * `CREATE TABLE table_name (column1 datatype constraints, ...)`
    * Specifying Primary Keys, Foreign Keys, `NOT NULL`, `UNIQUE`, `DEFAULT`, `CHECK`, `AUTO_INCREMENT`.
* **HackerRank Questions:** (Conceptual, often provided schemas)
    * Understanding table structure is key for all problems.
* **Interview Questions:**
    1. What is the primary purpose of the `CREATE TABLE` statement?
    2. List the essential components you need to specify when creating a table.
    3. How do you define a Primary Key during table creation?
    4. How do you define a Foreign Key that references another table's Primary Key?
    5. Give an example of creating a table with `NOT NULL` and `DEFAULT` constraints.
    6. What happens if you try to create a table with the same name as an existing table?
    7. Can you add a comment to a table or column during creation?
    8. What is the difference between column-level constraints and table-level constraints?
    9. How would you create a table that stores information about books, including title, author, publication year, and a unique ISBN?
    10. What is a "temporary table," and how is it created?

### • ALTER TABLE

* **Subtopics:**
    * Modifying an existing table structure.
    * `ADD COLUMN`: Add new column.
    * `DROP COLUMN`: Remove existing column.
    * `MODIFY COLUMN`/`ALTER COLUMN`: Change data type or constraints of a column.
    * `RENAME COLUMN`: Rename a column.
    * `ADD CONSTRAINT`/`DROP CONSTRAINT`: Add or remove constraints.
* **HackerRank Questions:** (Conceptual)
* **Interview Questions:**
    1. What is the `ALTER TABLE` statement used for?
    2. How would you add a new column named `email` with a `VARCHAR(100)` datatype to an existing `Employees` table?
    3. How do you remove an existing column from a table?
    4. Can you change the data type of an existing column using `ALTER TABLE`? What are the considerations?
    5. How do you add a `PRIMARY KEY` constraint to an existing column?
    6. What happens to existing data when you `DROP COLUMN`?
    7. How would you rename a column from `cust_id` to `customer_id`?
    8. Can `ALTER TABLE` statements be rolled back?
    9. What are the potential risks or impacts of running `ALTER TABLE` on a production database?
    10. How would you add a `NOT NULL` constraint to an existing column that already contains `NULL` values?

### • DROP TABLE

* **Subtopics:**
    * Deletes an entire table, including its data, structure, indexes, and constraints.
    * Irreversible in most cases without a backup.
* **HackerRank Questions:** (Conceptual)
* **Interview Questions:**
    1. What is the effect of the `DROP TABLE` statement?
    2. Can `DROP TABLE` be reversed? What precautions should be taken?
    3. What happens to associated indexes and constraints when you `DROP TABLE`?
    4. How does `DROP TABLE` differ from `DELETE FROM table_name` (without a WHERE clause)?
    5. What is the impact of `DROP TABLE` on Foreign Key relationships?
    6. When would you use `DROP TABLE`?
    7. Can you drop a table if it is currently being used by another session? (Varies by RDBMS, often locked).
    8. What is the syntax for dropping a table?
    9. What are the security implications of granting `DROP` privileges?
    10. How would you drop a table only if it exists, without throwing an error?

### • RENAME TABLE

* **Subtopics:**
    * Changes the name of an existing table.
    * Syntax varies slightly by RDBMS (e.g., `RENAME TABLE old_name TO new_name` or `ALTER TABLE old_name RENAME TO new_name`).
* **HackerRank Questions:** (Conceptual)
* **Interview Questions:**
    1. What is `RENAME TABLE` used for?
    2. How would you rename a table from `Customers` to `Clients`?
    3. What happens to views, stored procedures, or foreign keys that reference the old table name?
    4. Is `RENAME TABLE` a DDL or DML command?
    5. Are there any database-specific considerations when renaming tables?
    6. What are the potential impacts of renaming a table in a production environment?
    7. Does renaming a table affect its data?
    8. Can you rename a table that is currently locked or in use?
    9. What is the benefit of renaming tables rather than dropping and recreating them?
    10. Is `RENAME TABLE` a transactional operation?

### • TRUNCATE TABLE

* **Subtopics:**
    * Removes all rows from a table, but keeps the table structure, indexes, and constraints.
    * Faster than `DELETE` (without `WHERE`) for large tables.
    * Resets `AUTO_INCREMENT` counter (in most RDBMS).
    * Non-transactional (cannot be rolled back in most RDBMS).
* **HackerRank Questions:** (Conceptual)
* **Interview Questions:**
    1. What is the purpose of `TRUNCATE TABLE`?
    2. How does `TRUNCATE TABLE` differ from `DELETE FROM table_name`?
    3. Is `TRUNCATE TABLE` a DDL or DML command? Why?
    4. Can `TRUNCATE TABLE` be rolled back? Explain.
    5. What happens to the `AUTO_INCREMENT` counter after `TRUNCATE TABLE`?
    6. Does `TRUNCATE TABLE` log each row deletion? Why is this significant for performance?
    7. What are the implications of `TRUNCATE TABLE` on Foreign Key constraints?
    8. When would you choose `TRUNCATE TABLE` over `DELETE`?
    9. What privileges are required to execute `TRUNCATE TABLE`?
    10. Describe a scenario where `TRUNCATE TABLE` is the most efficient way to clear data.

## 14. Data Manipulation Language (DML)

### • INSERT INTO

* **Subtopics:**
    * Adds new rows of data into a table.
    * Specifying all column values in order.
    * Specifying specific columns.
    * Inserting multiple rows.
    * `INSERT INTO ... SELECT ...` (inserting results of a query).
* **HackerRank Questions:** (Not explicitly tested in the interactive environment, but fundamental to populating data)
* **Interview Questions:**
    1. What is the purpose of the `INSERT INTO` statement?
    2. How do you insert a single row into a table, providing values for all columns?
    3. How do you insert a single row, specifying values for only certain columns?
    4. Can you insert multiple rows with one `INSERT` statement? How?
    5. Explain `INSERT INTO ... SELECT ...`. When is this useful?
    6. What happens if you try to insert a value that violates a `NOT NULL` constraint?
    7. How does `INSERT` handle `AUTO_INCREMENT` columns?
    8. Can `INSERT` statements be rolled back?
    9. What are the performance considerations when inserting a very large number of rows?
    10. How would you insert a new employee record, ensuring the `hire_date` is the current date and time?

### • UPDATE

* **Subtopics:**
    * Modifies existing data in a table.
    * `SET` clause specifies columns and new values.
    * `WHERE` clause specifies which rows to update.
    * Updating multiple columns.
    * Using subqueries in `UPDATE`.
* **HackerRank Questions:** (Not explicitly tested, but understanding data modification is crucial)
* **Interview Questions:**
    1. What is the purpose of the `UPDATE` statement?
    2. How do you update a single column for a specific row?
    3. How do you update multiple columns for multiple rows?
    4. What happens if you omit the `WHERE` clause in an `UPDATE` statement?
    5. Can you use a subquery in the `SET` clause of an `UPDATE` statement? Give an example.
    6. Can `UPDATE` statements be rolled     back?
    7. What are the performance implications of updating a large number of rows?
    8. How would you increase the salary of all employees in the 'Sales' department by 10%?
    9. What are the risks of performing an `UPDATE` without careful testing of the `WHERE` clause?
    10. Can you update a column based on a value from another table using a `JOIN` within the `UPDATE` statement?

### • DELETE

* **Subtopics:**
    * Removes rows from a table.
    * `WHERE` clause specifies which rows to delete.
    * Deleting all rows.
    * Using subqueries in `DELETE`.
* **HackerRank Questions:** (Not explicitly tested, but understanding data modification is crucial)
* **Interview Questions:**
    1. What is the purpose of the `DELETE` statement?
    2. How do you delete specific rows from a table?
    3. What happens if you omit the `WHERE` clause in a `DELETE` statement?
    4. Can `DELETE` statements be rolled back?
    5. What is the difference between `DELETE` and `TRUNCATE`?
    6. How do Foreign Key constraints affect `DELETE` operations (e.g., `ON DELETE CASCADE`)?
    7. What are the performance implications of deleting a large number of rows?
    8. How would you delete all employees who have not been active for the last year?
    9. What are the security implications of granting `DELETE` privileges?
    10. Can you delete rows from one table based on conditions in another table?

### • MERGE (if supported)

* **Subtopics:**
    * Combines `INSERT`, `UPDATE`, and `DELETE` operations into a single statement.
    * Often used for synchronizing data between two tables (source and target).
    * Available in Oracle, SQL Server, PostgreSQL (since 9.5), not directly in MySQL.
* **HackerRank Questions:** (Not commonly tested on HackerRank)
* **Interview Questions:**
    1. What is the `MERGE` statement used for?
    2. Which DML operations can be performed using a single `MERGE` statement?
    3. In which database systems is `MERGE` commonly supported?
    4. When would you use `MERGE` over separate `INSERT`, `UPDATE`, and `DELETE` statements?
    5. Explain the `WHEN MATCHED` and `WHEN NOT MATCHED` clauses in `MERGE`.
    6. Can `MERGE` statement be rolled back?
    7. What are the advantages of using `MERGE` for data synchronization?
    8. Provide a simple example of a `MERGE` statement for updating or inserting customer data.
    9. What are the performance benefits and potential complexities of `MERGE`?
    10. Can you include a `WHERE` clause within the `WHEN MATCHED` or `WHEN NOT MATCHED` actions of a `MERGE` statement?

## 15. Transaction Control Language (TCL)

### • COMMIT

* **Subtopics:**
    * Makes all changes performed within a transaction permanent in the database.
    * Releases any locks held by the transaction.
* **HackerRank Questions:** (Conceptual)
* **Interview Questions:**
    1. What is the purpose of the `COMMIT` command?
    2. When should you issue a `COMMIT` statement?
    3. What happens to changes made within a transaction if `COMMIT` is not executed?
    4. Does `COMMIT` implicitly close a transaction?
    5. What are the effects of `COMMIT` on database performance and concurrency?
    6. Can DDL statements be committed explicitly?
    7. Explain how `COMMIT` ensures the durability aspect of ACID properties.
    8. What is "auto-commit" mode, and how does it affect explicit `COMMIT` statements?
    9. If multiple users are modifying the same data, how does `COMMIT` impact their view of the data?
    10. What is a "point of no return" in a transaction related to `COMMIT`?

### • ROLLBACK

* **Subtopics:**
    * Undoes all changes made during the current transaction.
    * Restores the database to its state before the transaction began.
    * Releases any locks.
* **HackerRank Questions:** (Conceptual)
* **Interview Questions:**
    1. What is the purpose of the `ROLLBACK` command?
    2. When would you use `ROLLBACK`? Give an example scenario.
    3. What happens to changes made within a transaction if `ROLLBACK` is executed?
    4. Can DDL statements be rolled back? Explain.
    5. How does `ROLLBACK` contribute to the atomicity of ACID properties?
    6. If a transaction includes both `INSERT` and `UPDATE` statements, what happens to both if `ROLLBACK` is issued?
    7. Are there any limitations to `ROLLBACK` (e.g., after a `COMMIT`)?
    8. What is the difference between a `ROLLBACK` and a `SAVEPOINT` rollback?
    9. What happens to database locks when a `ROLLBACK` occurs?
    10. Describe a situation where `ROLLBACK` is crucial for data integrity.

### • SAVEPOINT

* **Subtopics:**
    * Sets a named point within a transaction to which you can roll back.
    * Allows partial transaction rollback.
* **HackerRank Questions:** (Conceptual)
* **Interview Questions:**
    1. What is a `SAVEPOINT` used for?
    2. How does `SAVEPOINT` differ from `COMMIT` and `ROLLBACK`?
    3. Can you roll back to a specific `SAVEPOINT` without ending the entire transaction?
    4. Give a practical scenario where `SAVEPOINT` would be beneficial.
    5. What happens to subsequent `SAVEPOINT`s if you roll back to an earlier `SAVEPOINT`?
    6. Are `SAVEPOINT`s supported by all major RDBMS?
    7. What is the scope of a `SAVEPOINT`?
    8. Can you have multiple `SAVEPOINT`s within a single transaction?
    9. How does `SAVEPOINT` relate to nested transactions (if applicable to RDBMS)?
    10. Explain the process of creating a `SAVEPOINT` and then rolling back to it.

### • SET TRANSACTION

* **Subtopics:**
    * Sets the transaction characteristics for the current transaction.
    * Isolation levels (`READ UNCOMMITTED`, `READ COMMITTED`, `REPEATABLE READ`, `SERIALIZABLE`).
    * Read/write mode (`READ ONLY`, `READ WRITE`).
* **HackerRank Questions:** (Conceptual, highly advanced for freshers)
* **Interview Questions:**
    1. What is `SET TRANSACTION` used for?
    2. What are "isolation levels" in the context of transactions?
    3. Name and briefly describe the four standard isolation levels.
    4. What is the default isolation level in most database systems?
    5. Why are isolation levels important for concurrent access?
    6. Explain "dirty read," "non-repeatable read," and "phantom read" phenomena.
    7. Which isolation level prevents all three of these phenomena?
    8. What is the trade-off when choosing a higher isolation level?
    9. When would you set a transaction to `READ ONLY`?
    10. How does `SET TRANSACTION` contribute to the consistency and isolation aspects of ACID properties?

## 16. Data Control Language (DCL)

### • GRANT

* **Subtopics:**
    * Assigns database object privileges to users or roles.
    * Common privileges: `SELECT`, `INSERT`, `UPDATE`, `DELETE`, `CREATE`, `DROP`, `ALTER`, `EXECUTE`.
    * `WITH GRANT OPTION`: Allows the recipient to grant the privilege to others.
* **HackerRank Questions:** (Conceptual)
* **Interview Questions:**
    1. What is the purpose of the `GRANT` command?
    2. How do you grant `SELECT` permission on a specific table to a user?
    3. How do you grant all permissions on a database to a user?
    4. What does `WITH GRANT OPTION` mean when granting privileges?
    5. Can you grant privileges on specific columns of a table?
    6. What are the security implications of granting too many privileges?
    7. How would you grant a user permission to execute a stored procedure?
    8. What is the difference between `GRANT` and creating a new user?
    9. What happens if you try to `GRANT` a privilege that you don't possess?
    10. Explain a scenario where fine-grained `GRANT` control is necessary.

### • REVOKE

* **Subtopics:**
    * Removes previously granted privileges from users or roles.
    * `GRANT OPTION FOR`: Revokes the ability to grant a privilege.
    * `CASCADE`: Revokes the privilege from others who received it through the revoked user.
* **HackerRank Questions:** (Conceptual)
* **Interview Questions:**
    1. What is the purpose of the `REVOKE` command?
    2. How do you revoke `INSERT` permission on a table from a user?
    3. What happens if you revoke a privilege that was granted `WITH GRANT OPTION`?
    4. Explain the `CASCADE` option in `REVOKE`.
    5. What is the difference between `REVOKE` and `DENY` (if applicable to RDBMS)?
    6. Can you revoke a privilege from a role?
    7. What are the best practices for managing permissions to avoid security vulnerabilities?
    8. How would you revoke all privileges a user has on a specific table?
    9. Does `REVOKE` immediately affect active sessions? (Varies by RDBMS)
    10. Describe a scenario where `REVOKE` is essential for maintaining database security.

### • Roles and Privileges

* **Subtopics:**
    * **Privileges:** Specific permissions (e.g., `SELECT`, `INSERT`).
    * **Roles:** Collections of privileges that can be assigned to users. Simplifies permission management.
    * Granting roles to users.
    * Revoking roles from users.
* **HackerRank Questions:** (Conceptual)
* **Interview Questions:**
    1. What is the difference between a "privilege" and a "role" in SQL?
    2. Why are roles beneficial for managing database security?
    3. How do you create a new role?
    4. How do you grant privileges to a role?
    5. How do you assign a role to a user?
    6. Can a user have multiple roles?
    7. What happens to a user's permissions if a privilege is revoked from a role they are assigned to?
    8. What are some common built-in roles in SQL Server or Oracle?
    9. Describe a real-world scenario where using roles significantly simplifies security administration.
    10. What are the best practices for designing and implementing a role-based access control (RBAC) system in a database?

## 17. Normalization

### • What is Normalization?

* **Subtopics:**
    * A systematic approach to organizing the columns and tables of a relational database.
    * Reduces data redundancy and improves data integrity.
    * Divides large tables into smaller, related tables.
* **HackerRank Questions:** (Conceptual, designing correct schemas for problems implicitly relies on understanding normalization)
* **Interview Questions:**
    1. What is database normalization?
    2. What are the primary goals of normalization?
    3. Why is reducing data redundancy important?
    4. How does normalization improve data integrity?
    5. What are "update anomalies," "insertion anomalies," and "deletion anomalies"?
    6. What are the advantages of a normalized database?
    7. Are there any disadvantages to normalization?
    8. Who introduced the concept of normalization?
    9. What is a "functional dependency" in the context of normalization?
    10. Explain the general process of normalizing a database.

### • Objectives of Normalization

* **Subtopics:**
    * Eliminate redundant data.
    * Ensure data dependencies make sense (data is stored logically).
    * Reduce data modification anomalies (insertion, update, deletion anomalies).
    * Improve data consistency.
    * Make database design more flexible and scalable.
* **HackerRank Questions:** (Conceptual)
* **Interview Questions:**
    1. List at least three objectives of normalization.
    2. How does normalization help in maintaining data consistency?
    3. Explain how normalization prevents insertion anomalies with an example.
    4. Explain how normalization prevents update anomalies with an example.
    5. Explain how normalization prevents deletion anomalies with an example.
    6. What does it mean for data dependencies to "make sense"?
    7. How does normalization contribute to database design flexibility?
    8. Is the goal of normalization to always achieve the highest possible normal form? Why or why not?
    9. What role does data integrity play in the objectives of normalization?
    10. How does normalization facilitate concurrent access to data?

### • Types:

* **1NF (First Normal Form)**
    * **Subtopics:**
        * Eliminate repeating groups in individual tables.
        * Each column must contain atomic (single, indivisible) values.
        * Each record must be unique (Primary Key exists).
    * **HackerRank Questions:** (Conceptual)
    * **Interview Questions:**
        1. What are the rules for a table to be in First Normal Form (1NF)?
        2. What does "atomic value" mean in 1NF? Give an example of a non-atomic value.
        3. How do you achieve 1NF if a table has repeating groups?
        4. Why is a primary key required for 1NF?
        5. Give an example of a table that is not in 1NF and explain how to convert it.
        6. What anomalies can still exist in a table that is only in 1NF?
        7. Is 1NF always the first step in normalization?
        8. What are the benefits of achieving 1NF?
        9. How does 1NF relate to the concept of unique rows?
        10. Can a table be considered normalized if it's not even in 1NF?

* **2NF (Second Normal Form)**
    * **Subtopics:**
        * Must be in 1NF.
        * No partial dependencies: All non-key attributes must be fully dependent on the entire Primary Key (especially for composite keys).
    * **HackerRank Questions:** (Conceptual)
    * **Interview Questions:**
        1. What are the rules for a table to be in Second Normal Form (2NF)?
        2. Explain "partial dependency" with an example.
        3. How do you resolve a partial dependency to achieve 2NF?
        4. Why is 2NF important for reducing update anomalies?
        5. Give an example of a table that is in 1NF but not in 2NF, and explain how to normalize it to 2NF.
        6. What type of Primary Key is most relevant when discussing 2NF?
        7. What anomalies can still exist in a table that is only in 2NF?
        8. How does 2NF improve data integrity?
        9. Can a table with a single-column Primary Key ever violate 2NF? Why or why not?
        10. Describe the impact of not achieving 2NF on data consistency.

* **3NF (Third Normal Form)**
    * **Subtopics:**
        * Must be in 2NF.
        * No transitive dependencies: Non-key attributes must not be dependent on other non-key attributes.
    * **HackerRank Questions:** (Conceptual)
    * **Interview Questions:**
        1. What are the rules for a table to be in Third Normal Form (3NF)?
        2. Explain "transitive dependency" with an example.
        3. How do you resolve a transitive dependency to achieve 3NF?
        4. Why is 3NF important for reducing insertion and deletion anomalies?
        5. Give an example of a table that is in 2NF but not in 3NF, and explain how to normalize it to 3NF.
        6. What is the practical significance of reaching 3NF in most business applications?
        7. What is the "Boyce-Codd Normal Form" and how does it relate to 3NF?
        8. Can a table still have redundancy after reaching 3NF?
        9. How does 3NF contribute to database flexibility?
        10. What are some common real-world scenarios where transitive dependencies might occur?

* **BCNF (Boyce-Codd Normal Form)**
    * **Subtopics:**
        * Stricter than 3NF.
        * Every determinant must be a candidate key.
        * Addresses anomalies in tables with multiple overlapping candidate keys.
    * **HackerRank Questions:** (Conceptual, often more theoretical for freshers)
    * **Interview Questions:**
        1. What are the rules for a table to be in Boyce-Codd Normal Form (BCNF)?
        2. How does BCNF differ from 3NF?
        3. When might a table be in 3NF but not in BCNF? Provide an example.
        4. What is a "determinant" in the context of BCNF?
        5. Why is BCNF considered a stronger form of normalization than 3NF?
        6. Are all tables that are in BCNF also in 3NF, 2NF, and 1NF?
        7. Is it always necessary to achieve BCNF in database design? Explain.
        8. What are the potential drawbacks of over-normalizing to BCNF?
        9. How does BCNF handle the problem of overlapping candidate keys?
        10. Give a real-world example where BCNF would be important for data integrity.

### • Denormalization

* **Subtopics:**
    * Intentionally introducing redundancy into a database.
    * Opposite of normalization.
    * Done to improve query performance, especially for read-heavy operations.
    * Often involves adding redundant columns or combining tables.
* **HackerRank Questions:** (Conceptual)
* **Interview Questions:**
    1. What is denormalization?
    2. Why would you choose to denormalize a database?
    3. What are the main advantages of denormalization?
    4. What are the main disadvantages of denormalization?
    5. When     would you typically apply denormalization in database design?
    6. Give an example of a common denormalization technique.
    7. How does denormalization impact data integrity?
    8. What measures can be taken to mitigate the risks of denormalization?
    9. Describe a scenario where denormalization would be a sensible design choice.
    10. What is the trade-off between normalization and denormalization in terms of performance and data integrity?
