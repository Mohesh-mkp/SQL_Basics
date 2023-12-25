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
