##MySQL questions.
**How to join related tables?**
2 types: inner and outer

<a href="https://www.khanacademy.org/computer-programming/sql-join-on-tables/5409956539006976
">try</a>

<a href="http://www.sqlbook.com/sql/sql-inner-join-examples-and-explanations/
">more</a>

**Aggregating data**

SUM(), MAX(), MIN()

**What is AUTOINCREMENT and when to use it?**

-

**CASE. How to use**

SELECT something, something2
CASE
    WHEN ___ THEN "____"
    WHEN ___ THEN "___"
    ELSE "___"
END
FROM

<a href="https://www.w3schools.com/sql/func_mysql_case.asp">more</a>

**Subqueries**
'SELECT column-names
  FROM table-name1
 WHERE value IN (SELECT column-name
                   FROM table-name2 
                  WHERE condition)'
                  
<a href="http://www.dofactory.com/sql/subquery">more</a>

<a href="https://www.khanacademy.org/computing/computer-programming/sql/more-advanced-sql-queries/p/querying-in-subqueries
">try</a>

**Indexing. What types and how to use?**

<a href="https://www.tutorialspoint.com/mysql/mysql-indexes.htm">more</a>

**LIKE. What result you expecting with LIKE usage?**

<a href="https://www.tutorialspoint.com/mysql/mysql-like-clause.htm">more</a>

**Differentiate between CHAR_LENGTH and LENGTH**

- CHAR_LENGTH, as the name suggests, returns the number of characters / character count. The LENGTH returns the number of bytes / bytes count. To count the Latin characters, both lengths are the same. To count Unicode and other encodings, the lengths are different.

<a href="http://www.careerride.com/MySQL-CHAR_LENGTH.aspx">more</a>

**What is sharding? What the difference between particioning?**
It is table separating: horizontal (better when you need whole rows of data) and vertical (better for column data needs)
Most of times sharding is good for working with multiple instances (when DB is working on more then one machine), while particioning fits to single-instance-DB

[source](https://hazelcast.com/glossary/sharding/)

**What sharding methods do you know?**
Hash sharding and range sharding.
Range means "id > 100 AND id <= 1000", "id > 1000 AND id <= 2000" etc
Hash means "hash contains NNNN", "hash contains XYZXYZ", "hash contains 717171"

[source](https://blog.yugabyte.com/how-data-sharding-works-in-a-distributed-sql-database/)
