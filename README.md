# LearnSqlForQA
This is a training and refresher for QA test engineer to Refresh.

a) select statements in sql

# select *
select * from customer

# select Count
Select COUNT(*) FROM CUSTOMERTypes

# little extra if you want to give the name for the count returned value you can put something like this

Select COUNT(*) cnt_CustomerTyoes FROM CUSTOMERTypes  // Will return column name as 
|cnt_CustomerTyoes|
|105              |

# select number of record that has the visible tab = true
Select COUNT(*) FROM Departments where DP_Visible = 1

|no column name|
|3             |

# select Distinct DP_VISIBLE
SELECT DP_Visible from departments

# select Distinct DP_VISIBLE
SELECT DP_Visible from departments

# Use case: when using an aggregrate function like count you will need to use GROUP_BY
# We want to get the dinstict value in the DP_Visible field. This tells us if we have 0 or 1 (true or false) and possibly can be Null so what would be valueable is to the see the count of each distint value
SELECT DISTINCT DP_Visible, COUNT (DP_Visible) cnt
FROM Departments
GOURP BY DB_Visible.

The given SQL query aims to count the distinct values in the DP_Visible field from the Departments table. 

SELECT DP_Visible, COUNT(DP_Visible) AS cnt
FROM Departments
GROUP BY DP_Visible;

# how to use is_null, if i am taking out integer and ido a query 

SELECT DP_Description, ISNULL(DP_Order,99999) 
FROM Departments ORDER BY 2

# IF YOU ARE Tryig to concatinate together, if you need to do that then you have to use CAST

SELECT DP_Description, ISNULL(DP_Order,99999) 
FROM Departments ORDER BY 2



