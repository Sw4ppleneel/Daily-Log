# Started learning SQL using MySQL. 

Today's notes : 

SQL structured query language 

CRUD operations on SQL 

Create 
Read
Update
Delete 

Works on relational databases. (In tables)

Basic query :
Create database {name} 
#Creates  new database 
Drop database {name} 
#Deletes database

use {db-name} 

//
create table {table name}(

{name 1} {datatype} {constraint}
{name 2} {datatype} {constraint}
{name 3} {datatype} {constraint}
);
//

Constraints : 
NOT NULL - cannot be null 

Unique - must be unique 

PRIMARY KEY - both of the above. 
At end as
Primary key {var}

FOREIGN KEY ({variable}) references {table}({variable})

Default , if null fills default value 
{Salary int} default 25000 (constraint)

Check (inbuilt if) 
Check (age >= 18)

Constraints can be added explicitly	in the table at end.
As 

Constraint {variable} {constraint}

Select :

Select distinct {column} from {table}
Selects distinct elements from table column. 
Using * selects all column.

Clause : 

Clauses can be used together. 

Where 

To apply a condition , 
Select {column} from table 
Where {var} {condition} eg. City = mumbai AND marks > 80 .

Operators : 

AND and OR usage aata hoga bhai.  

Where marks between 80 and 90 . For a range.(both are inclusive) , 

IN , where city IN (“Mumbai” , ”Delhi”)
Selects if condition matches any from the list. 

NOT IN , obvious enough I hope. 

Limit clause , 
Limits number of rows.

Order By clause ,
Order by roll no ASC; // DESC 


Aggregate functions:
count()
max()
min()
sum()
avg()

Select max(marks)
From student_mks;

Group By clause , 
No of students from each city 
Select city , count(name)
From student 
Group by city;

Select variables and group by should be same.
