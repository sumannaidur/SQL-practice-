# **Module 2: Datatypes and Constraints**

This module delves into the essential building blocks of a well-designed table: datatypes and constraints. These two concepts work together to ensure data integrity, meaning the data in your database is accurate, consistent, and reliable.

### **1\. What are Datatypes?**

#### **Technical Explanation**

A **datatype** is an attribute that specifies the type of data that an object (like a column in a table) can hold. It defines the possible values for that column, the operations that can be performed on it, and how the data is stored in memory and on disk. When you create a table, you must assign a specific datatype to each of its columns.

For example, a column intended to store employee salaries should have a numeric datatype (like INT or DECIMAL), while a column for their names should have a character string datatype (like VARCHAR). Assigning the correct datatype is the first line of defense in maintaining data quality. Trying to insert text into a numeric column will result in an error.

#### **Real-Life Analogy: Labeled Containers**

Imagine you are organizing your kitchen pantry. You don't just throw everything onto the shelves randomly. You use specific containers for specific items:

* A tall, sealed glass jar for spaghetti (**a container for long, thin, dry things**).  
* A ceramic sugar bowl with a lid for sugar (**a container for fine, white granules**).  
* A liquid-tight bottle for olive oil (**a container for oils**).

In this analogy:

* The **containers are the columns** in your table.  
* The **labels on the containers ("Spaghetti," "Sugar," "Oil") are the datatypes**.  
* The **items you put inside are the actual data**.

You wouldn't pour olive oil into the sugar bowl—it's the wrong type of container for that kind of "data." A datatype in SQL works the same way; it's a rule that defines what kind of data can go into a column.

### **2\. Common Built-in Datatypes**

Different database systems might have slightly different names or variations for these types, but the concepts are universal.

| Datatype Category | Common Types | Description & Use Case | Syntax Example (in a CREATE TABLE statement) |
| :---- | :---- | :---- | :---- |
| **Character Strings** | VARCHAR(n) | Variable-length string. n is the maximum number of characters. Use for data with varying lengths like names or addresses. | LastName VARCHAR(50) |
|  | CHAR(n) | Fixed-length string. n is the exact number of characters. If the input is shorter, it's padded with spaces. Good for fixed-length codes like state abbreviations ('NY', 'CA'). | StateCode CHAR(2) |
|  | TEXT / CLOB | For very long variable-length text, like product descriptions or articles. | ProductDescription TEXT |
| **Numeric** | INT or INTEGER | Whole numbers (no decimals). Used for counts, quantities, or IDs. | Quantity INT |
|  | DECIMAL(p, s) | Fixed-point numbers, ideal for currency. p is total digits (precision), s is digits after decimal (scale). | Price DECIMAL(10, 2\) |
|  | FLOAT / REAL | Floating-point numbers for scientific calculations where absolute precision isn't as critical as in finance. | Measurement FLOAT |
| **Date & Time** | DATE | Stores the date (year, month, day). | HireDate DATE |
|  | TIME | Stores the time (hour, minute, second). | AppointmentTime TIME |
|  | TIMESTAMP | Stores both date and time. Often used for logging when a record was created or modified. | LastUpdated TIMESTAMP |
| **Boolean** | BOOLEAN | Stores TRUE or FALSE values. (Some systems like Oracle use NUMBER(1) or CHAR(1) to simulate this). | IsActive BOOLEAN |
| **Binary** | BLOB | Binary Large Object. Used for storing binary data like images, audio files, or video clips directly in the database (though often not recommended). | ProfilePicture BLOB |

### **3\. What are Constraints?**

#### **Technical Explanation**

A **constraint** is a rule enforced on a data column or set of columns to ensure the accuracy and reliability of the data. Constraints are used to limit the type of data that can go into a table. If any DML operation (like INSERT, UPDATE) violates a constraint, the operation is aborted. Constraints can be defined at the column level or the table level.

#### **Real-Life Analogy: Rules for a Parking Garage**

Think of a multi-level parking garage. It has rules to keep things orderly and functional:

* **Rule 1: Every spot has a unique number (A1, A2, B1).** You can't have two spots labeled A1. This is a **UNIQUE** or **PRIMARY KEY** constraint.  
* **Rule 2: You cannot park in a spot reserved for "Handicapped Parking" unless you have a valid permit.** This is a **CHECK** constraint (e.g., CHECK (HasPermit \= TRUE)).  
* **Rule 3: The "Reserved for CEO" spot cannot be empty; the CEO's car must be there.** This is a conceptual parallel to a **NOT NULL** constraint.  
* **Rule 4: If you have a monthly pass, it must correspond to a valid customer account in the office's records.** You can't have a pass for a non-existent customer. This is a **FOREIGN KEY** constraint.

These rules (constraints) prevent chaos and ensure the garage (table) operates correctly.

### **4\. Common SQL Constraints**

| Constraint | Description | Column-Level Syntax | Table-Level Syntax |
| :---- | :---- | :---- | :---- |
| **NOT NULL** | Ensures a column cannot have a NULL (empty) value. | EmployeeID INT NOT NULL | (Not applicable) |
| **UNIQUE** | Ensures all values in a column (or set of columns) are different. | Email VARCHAR(100) UNIQUE | CONSTRAINT uc\_Email UNIQUE (Email) |
| **PRIMARY KEY** | A combination of NOT NULL and UNIQUE. Uniquely identifies each record in a table. A table can have only one Primary Key. | ProductID INT PRIMARY KEY | CONSTRAINT pk\_ProductID PRIMARY KEY (ProductID) |
| **FOREIGN KEY** | Uniquely identifies a record in another table, creating a link between the two. Enforces "referential integrity." | CustomerID INT REFERENCES Customers(CustomerID) | CONSTRAINT fk\_CustomerID FOREIGN KEY (CustomerID) REFERENCES Customers(CustomerID) |
| **CHECK** | Ensures the values in a column satisfy a specific condition. | Salary DECIMAL(10,2) CHECK (Salary \> 0\) | CONSTRAINT chk\_Salary CHECK (Salary \> 0\) |
| **DEFAULT** | Sets a default value for a column when no value is specified. | Status VARCHAR(10) DEFAULT 'Active' | (Not applicable) |

### **🧠 HackerRank-Style Practice Questions**

*Assume you are creating the following tables for these challenges:*

CREATE TABLE Employees (  
    EmployeeID INT PRIMARY KEY,  
    FirstName VARCHAR(50) NOT NULL,  
    LastName VARCHAR(50) NOT NULL,  
    Email VARCHAR(100) UNIQUE,  
    HireDate DATE DEFAULT CURRENT\_DATE,  
    Salary DECIMAL(10, 2\) CHECK (Salary \>= 25000),  
    DepartmentID INT  
);

CREATE TABLE Departments (  
    DepartmentID INT PRIMARY KEY,  
    DepartmentName VARCHAR(50) NOT NULL UNIQUE  
);

1. **Challenge:** Write a CREATE TABLE statement for a Products table with ProductID (integer, primary key), ProductName (variable string up to 100 chars, cannot be null), Price (decimal, must be greater than 0), and StockQuantity (integer, defaults to 0).  
2. **Challenge:** Add a foreign key constraint to the Employees table that links DepartmentID to the DepartmentID in the Departments table.  
3. **Challenge:** Write an INSERT statement that will **fail** because it violates the CHECK constraint on the Employees Salary column.  
4. **Challenge:** Write an INSERT statement that will **fail** because it violates the UNIQUE constraint on the Employees Email column (assuming another employee with that email already exists).  
5. **Challenge:** Write an INSERT statement for the Employees table that relies on the DEFAULT value for the HireDate column.  
6. **Challenge:** You need to add a JobTitle column (variable string up to 50 characters) to the Employees table. Write the ALTER TABLE statement.  
7. **Challenge:** Write a CREATE TABLE statement for an Orders table. It should have an OrderID (PK), OrderDate (defaults to today), CustomerID (links to a Customers table), and an OrderStatus column that can only be one of the following values: 'Pending', 'Shipped', 'Delivered'.  
8. **Challenge:** Write an INSERT statement that will **fail** because it violates the NOT NULL constraint on the Departments DepartmentName column.  
9. **Challenge:** Write an ALTER TABLE statement to add a CHECK constraint to the Products table ensuring that StockQuantity is never negative.  
10. **Challenge:** A company decides that every employee must belong to a department. Write an ALTER TABLE statement to enforce this rule on the Employees table's DepartmentID column.  
11. **Challenge:** Write a CREATE TABLE statement for a Reviews table. It needs a ReviewID (PK), ProductID (FK to Products), Rating (integer from 1 to 5), and ReviewerName (defaults to 'Anonymous').

### **🎙️ Interview Questions**

#### **Basic Level**

1. **Q:** What is a datatype?  
   * **A:** It's a label for a column that defines what kind of data it can store, like numbers, text, or dates.  
2. **Q:** Why is it important to choose the correct datatype?  
   * **A:** It ensures data integrity by preventing wrong data types from being entered, optimizes storage space, and makes queries more efficient.  
3. **Q:** What's the difference between CHAR and VARCHAR?  
   * **A:** CHAR is fixed-length, so it always uses the same amount of storage space, padding with spaces if needed. VARCHAR is variable-length, so it only uses space for the characters you actually store. VARCHAR is generally preferred unless the data length is always the same (e.g., state codes).  
4. **Q:** What is a constraint?  
   * **A:** It's a rule enforced on the data in a table to ensure its accuracy and reliability.  
5. **Q:** What is a PRIMARY KEY?  
   * **A:** It's a constraint that uniquely identifies each record in a table. It must contain unique values and cannot contain NULL values.  
6. **Q:** Can a table have more than one PRIMARY KEY?  
   * **A:** No, a table can have only one primary key. However, a primary key can consist of multiple columns (this is called a composite primary key).  
7. **Q:** What does the NOT NULL constraint do?  
   * **A:** It ensures that a column cannot be left empty; it must have a value.  
8. **Q:** What is the purpose of the DEFAULT constraint?  
   * **A:** It provides a default value for a column if no value is specified during an INSERT operation.  
9. **Q:** What is a FOREIGN KEY?  
   * **A:** It's a key used to link two tables together. It's a field (or collection of fields) in one table that refers to the PRIMARY KEY in another table.  
10. **Q:** What is the UNIQUE constraint?  
    * **A:** It ensures that all values in a column are different from one another. Unlike a primary key, it can allow one NULL value.

#### **Intermediate Level**

11. **Q:** Explain the difference between a PRIMARY KEY and a UNIQUE constraint.  
    * **A:** Both enforce uniqueness. However, a table can have only one PRIMARY KEY, but multiple UNIQUE constraints. Also, a PRIMARY KEY cannot have NULL values, whereas a UNIQUE constraint can typically accept one NULL value.  
12. **Q:** What is referential integrity and how is it enforced?  
    * **A:** Referential integrity is the rule that a foreign key value must match an existing primary key value in the referenced table. It's enforced by the database using FOREIGN KEY constraints. This prevents "orphan" records, like an order for a customer who doesn't exist.  
13. **Q:** What is a CHECK constraint? Give a practical example.  
    * **A:** It's a rule that limits the value range that can be placed in a column. For example, on a Salary column, you could have CHECK (Salary \> 0), or on a Gender column, CHECK (Gender IN ('M', 'F', 'Other')).  
14. **Q:** When would you use DECIMAL instead of FLOAT?  
    * **A:** You would use DECIMAL for exact numeric values where precision is critical, such as financial data (money, salaries, account balances). FLOAT is used for approximate numeric values, like scientific measurements, where a tiny loss of precision is acceptable.  
15. **Q:** Can a foreign key be NULL?  
    * **A:** Yes, a foreign key column can be NULL. This would imply that the record is not related to any record in the parent table. For example, an employee might not yet be assigned to a department, so their DepartmentID foreign key could be NULL.  
16. **Q:** What is a composite key?  
    * **A:** A composite key is a key (primary, unique, or foreign) that is made up of two or more columns combined. It's used when one column alone is not sufficient to uniquely identify a record.  
17. **Q:** What happens if you try to insert a row that violates a constraint?  
    * **A:** The database will reject the INSERT statement and return an error message describing the constraint violation. The transaction is rolled back, and the table remains unchanged.  
18. **Q:** What is the difference between a column-level constraint and a table-level constraint?  
    * **A:** A column-level constraint is defined as part of the column definition itself and applies only to that one column. A table-level constraint is defined separately from any column definition and can apply to one or more columns (which is necessary for composite keys).

#### **Advanced Level**

19. **Q:** How can constraints impact database performance?  
    * **A:** Constraints can slightly slow down DML operations (INSERT, UPDATE, DELETE) because the database must perform checks to ensure the rules are not violated. For example, inserting into a table with many foreign keys requires lookups in other tables. However, this overhead is almost always a worthwhile trade-off for ensuring data integrity. For read operations (SELECT), constraints like primary keys create indexes that dramatically *improve* performance.  
20. **Q:** What are ON DELETE CASCADE and ON DELETE SET NULL?  
    * **A:** These are actions that can be specified on a FOREIGN KEY constraint to define what happens to the child records when a parent record is deleted.  
      * **ON DELETE CASCADE**: If the parent record is deleted, all corresponding child records are also automatically deleted.  
      * **ON DELETE SET NULL**: If the parent record is deleted, the foreign key fields in the corresponding child records are set to NULL.  
21. **Q:** Can you temporarily disable a constraint? Why would you want to?  
    * **A:** Yes, in most RDBMSs (like Oracle or SQL Server), you can disable and later re-enable constraints. You might do this during a large bulk data load to speed up the process, as the constraints are not checked for each individual row. However, you must be certain the data being loaded is clean, and you typically have to re-validate the constraint against the entire table when you re-enable it.  
22. **Q:** What is a BLOB datatype, and what are the pros and cons of using it to store files in a database?  
    * **A:** A BLOB (Binary Large Object) is a datatype for storing large binary data like images or documents.  
      * **Pros:** Data and metadata are stored together transactionally; backup and recovery processes include the files.  
      * **Cons:** It can significantly bloat the database size, which can slow down backups. It can also be less efficient than simply storing a file path (a VARCHAR) in the database and keeping the file on a dedicated file system.