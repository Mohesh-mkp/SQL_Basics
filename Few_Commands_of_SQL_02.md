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


__GROUP BY:__ 
