# Keys
To define special columns in the table we use the concept of key.    
They are of many types. A few of them are listed below;   
1. Primary Key
2. Foreign Key

### Primary Key:
- It's a column that holds unique values which is not similar to each other.
- A table can contain only one primary key.
- For example, In a student table id and roll number both are unique but we need to choose either of them as a primary key, whereas a Name that can be the same is not preferred to select as the primary key
- Primary key value can not be NULL, which means you can not put an empty value to the primary key holder row.

### Foreign Key:
- It's a column in a table that refers to a primary key.
- There can be multiple foreign keys present in a tale.
- These columns can have duplicate as well as NULL values.

# Constraints
Constraints mean some rules for data in the table.    
A few of the constraints are;     

- NOT NULL -> This specifies that the column value should not contain any null values.
- UNIQUE -> This specifies that the column value always contains a unique value that should not repeat
- PRIMARY KEY -> This specifies that the column value always contains a unique value that should not repeat as well as it should not contain null value
- FOREIGN KEY -> A link between two different table
    ```
    Example of Foreign key:

    CREATE TABLE student(
    cust_id INT,
    FOREIGN KEY (cust_id) references customer(id)  # Here the customer is another table and id is a column of that table
    );
    ```
- DEFAULT -> sets the default value of a column
    ```
    Example:
    salary INT DEFAULT 25000

    Here if the column value was not entered then it will take the default value and will not put any empty value
    ```
- CHECK -> To limit the value in the column
    ```
    CREATE TABEL emp(
    age INT CHECK(age >= 18)
    );
    ```




