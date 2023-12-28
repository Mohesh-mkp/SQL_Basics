## Table related Queries (Continued from previous)

__DISTINCT:__ Used to display the unique values from repeated data of Columns.
If a data table consists of multiple times of a particular city or data, then with the below command it will list out the unique city or data available in the table.    

_Syntax:_ SELECT DISTINCT col_name FROM table_name;
```
Example:
SELECT DISTINCT city FROM emp;
```
__WHERE:__ Used to define some conditions     

_Syntax:_  SELECT col1_name, col2_name FROM table_name WHERE conditions;
```
Example:

SELECT city, salary FROM mnc WHERE salary > 100000;

```

__LIMIT:__ To list out a limited number of data from the database.

_Syntax:_ SELECT col1_name, col2_name FROM tab;e_name LIMIT number;

_Example;_

![image](https://github.com/Mohesh-mkp/SQL_Basics/assets/101304247/77447d2e-8a7e-45f8-bf58-3fd79d2791fd)

![image](https://github.com/Mohesh-mkp/SQL_Basics/assets/101304247/1e1c99a9-aa50-4255-b686-df86c93a0aca)



__ORDER BY:__ To list out data in ascending(ASC) or descending(DESC) order.     

_Syntax:_ SELECT col_name FROM table_name ORDER BY col_name ASC        # for ascending       

_Syntax:_ SELECT col_name FROM table_name ORDER BY col_name DESC        # for descending

_Example:_

![image](https://github.com/Mohesh-mkp/SQL_Basics/assets/101304247/ec50e9b4-6288-48e6-bf56-0c1d5d3e570f)

![image](https://github.com/Mohesh-mkp/SQL_Basics/assets/101304247/c95395c2-9a31-4547-9590-98784e08f5dc)


__GROUP BY:__ To group the rows with the same values.   
```
Note:
Generally, we use group by with some aggregation function.
```
_Example:_    

![image](https://github.com/Mohesh-mkp/SQL_Basics/assets/101304247/d554e65d-52ec-4c44-966c-97b52202fbce)

![image](https://github.com/Mohesh-mkp/SQL_Basics/assets/101304247/50d45ea3-8608-4813-a793-416a444f5927)


## Practice Question:
- create a table of students and table consists of the following columns
    -  rollno
    -  Name
    -  marks
    -  City
- Write the query to find average marks in each city in ascending order

```
Solution:

CREATE DATABASE college;
USE college;

CREATE TABLE student(
rollno INT PRIMARY KEY,
name VARCHAR(50),
city VARCHAR(15),
marks INT
);

INSERT INTO student
(rollno, name, city, marks)
VALUES
(101, 'Karan', 'Pune', 67),
(102, 'John', 'Delhi', 69),
(103, 'Joseph', 'Mumbai', 79),
(104, 'Raghuram', 'Pune', 89),
(105, 'Veera', 'Punjab', 99),
(106, 'Yashwant', 'Delhi', 59);

SELECT city, avg(marks)
FROM student
GROUP BY city
ORDER BY city;

```
## Another Practice Question:
![image](https://github.com/Mohesh-mkp/SQL_Basics/assets/101304247/27aaa4d6-168c-4130-a1d1-5c3e82dcfa03)

```
Solution:
Note: After the creation of the database of the given example only the following code is to be written.

CREATE DATABASE customerPayment;
USE customerPayment;
CREATE TABLE payment(
customer_id INT PRIMARY KEY,
customer VARCHAR(50),
mode VARCHAR(15),
city VARCHAR(15)
);
INSERT INTO payment
(customer_id, customer, mode, city)
VALUES
(all data to be inserted inside);

SELECT mode, count(customer)
FROM payment
GROUP BY mode;

```








