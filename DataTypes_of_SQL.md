Few Data Types:    
![image](https://github.com/Mohesh-mkp/SQL_Basics/assets/101304247/b241cdb4-db4d-454d-bfb7-a6f4ced530ac)

### CHAR and VARCHAR:
To define a string in a variable we are using __CHAR and VARCHAR__ in SQL.    
__CHAR:__ string(0-255), can store characters of fixed length.  eg: CHAR(50)    
__VARCHAR:__ string(0-255), can store characters up to given length.  eg: VARCHAR(50).    

Seems like CHAR and VARCHAR same????     
No, The difference between CHAR and VARCHAR is,    
CHAR(50): This tells us that it will store elements of fixed length 50 and it is reserved. If there is space after the defined string in CHAR we can not use them for further.   
![image](https://github.com/Mohesh-mkp/SQL_Basics/assets/101304247/07d002cf-85d5-4437-a859-05d8f70f3cd2)    
Here, After entering PUNE there is space of 2-3 cells but CHAR makes them reserve and it's of no use. Hence memory management is not good.    

Whereas VARCHAR will store up to the given length and will efficiently use memory. If the string is PUNE then it will format the memory of the given length and save the memory for further.    
![image](https://github.com/Mohesh-mkp/SQL_Basics/assets/101304247/39eb8a01-5a32-4f7d-b791-a04ffb1e2b90)


__Note:__ That is the reason we will use VARCHAR to define a string element to use memory efficiently.    

### BLOB:
To store big strings like a file of data.    
string(0-65535), can store binary large objects. (BLOB 1000)    

