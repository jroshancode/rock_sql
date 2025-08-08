# rock_sql

I have used for learning and practice and prefer to you also. 
W3schools:- [ https://www.w3schools.com/sql/sql_exercises.asp] <br>
Codechef:- [ https://www.codechef.com/practice/sql-case-studies-topic-wise] <br> 
hackerrank:- [ https://www.hackerrank.com/domains/sql ] <br> 
sqlzoo  :- [https://sqlzoo.net/wiki/SQL_Tutorial ] <br> 
Geeksforgeeks :- [ https://www.geeksforgeeks.org/sql/sql-exercises/] <br> 
Leetcode :- https://leetcode.com/studyplan/top-sql-50/<br> 
        
____________________________________



/*
Enter your query here.
*/

-- students => Id, Name,marks 

-- Grade => Grade, min_mark , max_Mark

-- grade lower than 8 
-- order by desc grade 

-- 8-10 => order by name



1. 2025 - 07 - 18
   https://www.kaggle.com/datasets/smayanj/e-commerce-transactions-dataset



In SQL, both subqueries and Common Table Expressions (CTEs) are mechanisms used to structure and manage complex queries, 
but they differ in their definition and usage.

Subquery
A subquery, also known as an inner query or nested query, is a SELECT statement embedded within another SQL query. 
It executes first, and its result is then used by the outer query. Subqueries can be used in various clauses, 
including SELECT, FROM, WHERE, HAVING, INSERT, UPDATE, and DELETE.

                    


# 2025 - 07 - 29 
https://www.kaggle.com/datasets/ravindrasinghrana/employeedataset


#2025 - 08 - 04 

https://leetcode.com/problems/delete-duplicate-emails/description/?envType=study-plan-v2&envId=top-sql-50


#2025 - 08 - 05 
https://leetcode.com/problems/delete-duplicate-emails/?envType=study-plan-v2&envId=top-sql-50

-- delete p1 from Person as p1 
-- join ( 
--     select email, min(id) as id from Person group by email
-- ) as etc

-- on etc.email = p1.email and p1.id <> etc.id


-- with etc as ( 
--     select email, min(id) as id from Person group by email
-- )

-- delete from Person where id not in( 
--     select id from etc
-- )


-- with etc as ( 
--     select min(id) as id from Person group by email
-- )

-- delete from Person where id not in( 
--     select id from etc
-- )


-- delete from Person where id not in( 
--     select * from ( 
--        select min(id) as id from Person group by email 
--        ) as etc
-- )

delete p1 from person as p1 , person as p2 
where p1.email = p2.email and p1.id >p2.id



#2025 - 08- 06

select * from train;
-- fetch the all records and count number of records for march months.
select *
from train where month(`Order Date`) = 3;

select * from housing_price;

select count(*)
from housing_price where SaleDate like "%March%";

select count(*)
from housing_price where  month(new_date) = 3;


# (YouTube Sports Channels Statistics) [https://www.kaggle.com/datasets/kanchana1990/youtube-sports-channels-statistics?resource=download]


# Feedback form 
[https://forms.gle/gERXp6iX8gJUjDBY6]
