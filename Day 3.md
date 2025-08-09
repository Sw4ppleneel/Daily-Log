Day 3 : 

# Subqueries :

Nested query :

Select name , marks
From {table name}
Where marks operator (subquery);

Select max(mks)
From ( select * from student  where city = "delhi”);

# SQL view :

Virtual table based on a table.

Create view as VIEW1
Select roll no , name from {base table}

Select * from view1; 

Droppig view 

Drop view view1;