### To create a database:
__CREATE DATABASE db_name;__   

This command is used for creating database with given name db_name, db_name can be changed to any name as college or project.   

To perform any action on database we are giveing command as __USE db_name;__   
This command gives us the permission or access to create table or fellow element require for database.   

### To create a table:
```
Syntax to create table:

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

