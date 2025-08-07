Moving on to day two : 

Today's notes : 

Having clause , is used for condition set on a group .

General order of clauses ,

Select col
From table-name
Where condition
Group by col
Having condition
Order by col

Update query in table

Update table-name
Set col 1 = val 1 , col 2 = val2
Where condition;

Delete operation ,

Delete from table-name
Where Condition

Cascading for FK

ON DELETE CASCADE
ON DELETE CASCADE , under foreign key definition, so deletes and updates are reflected	from main table to referencing	table.

Table related queries


Alter ( to change schema )

To sdd
Alter table table-name
Add column name datatype constraint

To drop
Alter table tablename
Drop column name

Rename ,
Alter table table-name
Rename to new-name

Change column
Alter table table-name
Change column old-name new-name newdatatype new-constraint.

Modify column , keep name	same
Alter table table-name
Modify column new-datatype new-constraint


SQL Joins

Used to join two tables or more in sql

Select {columns}
From tableA
Inner Join tableB
On tableA.col = tableB.col ;

Inner join both table common data
Left join left table all data , and overlap
Right join  right table all data and overlap.
Full join , joins all data and matching data.

In mysql use union command between left and right joins.

For left exclusive join

Where b.col IS NULL.

For right exclusive join

Where a.col is null.

Self join

Joins with own table

Select a.col as namevar, b.name
From table as a
Join table as b
On a.id = b.manager.id ;

Union
Select col from A
Union
Select col from B