# Commands with Structured steps

## Database Related Queries:

__CREATE DATABASE db_name;__   
```
This command is used for creating a database with a given name db_name, db_name can be changed to any name.
```

__CREATE DATABASE IF NOT EXISTS db_name;__   
```
This command is used to create a database if that is not present.
For example, we already have a database with the name college and if we run the previous command mistakenly,
then it will throw an error. However, with this command, it will throw a warning message stating that the database
will not be created since the name with the database already exists. 
```

__DROP DATABASE db_name;__
```
This command is used to delete the database.
```

__DROP DATABASE IF EXISTS db_name;__
```
This command is used to delete the database if it is present. For example, if a database is not present
and we try to delete that, then we will receive an error. So this command will help to skip the error and
instead of an error, it will throw a warning stating that the database does not exist.
```


__USE DATABASE;__
```
To perform any action on a database we are giving the command as __USE db_name;__      
This command gives us permission or access to create a table or fellow elements required for the database.   
```

__SHOW DATABASEs;__   
```
This command is used to show all the databases present in SQL Server.
```

__SHOW TABLES;__   
```
This command is used to show all the tables inside the databases.
```

## Table Related Queries
__CREATE TABLE tb_name (parameter inside);__

This command is used to create a table.
```
Syntax:

CREATE TABLE table_name (   
column_name1 datatype constraint,   
column_name2 datatype constraint,   
column_name3 datatype constraint,   
);

```
Example:    

CREATE TABLE student (    
  id INT Primary Key,    
  name VARCHAR(50),    
  age INT NOT NULL,   
);   

![image](https://github.com/Mohesh-mkp/SQL_Basics/assets/101304247/4223bb48-44d0-4649-a641-40817c0ac95e)

__SELECT col1, col2 FROM tb_name;__    
This command is used to view columns1 and column2 data from the table.   

__SELECT * FROM tb_name;__    
This command is used to view all columns from the table.   

__INSERT INTO tb_name(col1, col2) VALUES (col1_v1, col2_v2);__
This command is used to insert values to respective columns of the table.    
```
Syntax:

INSERT INTO tb_name
(column1_name, column2_name)

VALUES
(col1_val1, col2_val1)
(col1_val2, col2_val2)

```
Example:    
INSERT INTO student    
(id, name, age)     
VALUES      
(1,'RAM', 23),     
(2.'Karan', 34);      

NOTE: The order of columns and values needs to be considered.    
Also, we can add single data to the table like;
```
INSERT INTO student VALUES (3, 'RAVI', 25);
```

## Practice program:
![image](https://github.com/Mohesh-mkp/SQL_Basics/assets/101304247/b9de9620-16c4-40b0-b19b-0d27da8cda16)
```
CREATE DATABASE XYZ;
USE XYZ;
CREATE TABLE employee (
id INT PRIMARY KEY,
Name VARCHAR(50),
Salary INT
);

INSERT INTO employee
(id, Name, Salary)
VALUES
(1, 'adam', 25000),
(2, 'bob', 30000),
(3, 'casey', 40000);

SELECT * FROM employee;

```

