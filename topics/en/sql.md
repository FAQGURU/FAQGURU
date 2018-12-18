## SQL

[What is PRIMARY KEY?](#what-is-primary-key)

[Define a temp table ](#define-a-temp-table-)

[What is a view?](#what-is-a-view)

[What’s the difference between a local  temp table and a global temp table?](#whats-the-difference-between-a-local--temp-table-and-a-global-temp-table)

[What is blocking?](#what-is-blocking)

[What is the difference between WHERE clause and HAVING clause?](#what-is-the-difference-between-where-clause-and-having-clause)

[What is FOREIGN KEY?](#what-is-foreign-key)

[What is Normalization?](#what-is-normalization)

[How can a column with a default value be added to an existing table?](#how-can-a-column-with-a-default-value-be-added-to-an-existing-table)

[What is DEFAULT?](#what-is-default)

[What is the difference between inner and outer join?](#what-is-the-difference-between-inner-and-outer-join)

[Discuss INNER JOIN ON vs WHERE clause](#discuss-inner-join-on-vs-where-clause)

[What are the difference between clustered and a non-clustered index?](#what-are-the-difference-between-clustered-and-a-non-clustered-index)

[How do I perform an IF…THEN in an SQL SELECT?](#how-do-i-perform-an-ifthen-in-an-sql-select)

[Finding duplicate values in a SQL table](#finding-duplicate-values-in-a-sql-table)

[How does a hash table index work?](#how-does-a-hash-table-index-work)

[What are the advantages of using Stored Procedures?](#what-are-the-advantages-of-using-stored-procedures)

[What is Denormalization?](#what-is-denormalization)

[How to select first 5 records from a table?](#how-to-select-first-5-records-from-a-table)

[Define ACID Properties](#define-acid-properties)

[How a database index can help performance?](#how-a-database-index-can-help-performance)

[What is the difference between UNION and UNION ALL?	](#what-is-the-difference-between-union-and-union-all	)

[What is a cursor how does it work?](#what-is-a-cursor-how-does-it-work)

[How do I UPDATE from a SELECT in SQL Server?](#how-do-i-update-from-a-select-in-sql-server)

[What is the difference between “INNER JOIN” and “OUTER JOIN”?](#what-is-the-difference-between-inner-join-and-outer-join)

[Is table size reduced, when you delete data from the table?](#is-table-size-reduced-when-you-delete-data-from-the-table)

[Explain Function vs. Stored Procedure in SQL Server](#explain-function-vs-stored-procedure-in-sql-server)

[What are row constructors?](#what-are-row-constructors)

[What is the difference between JOIN and UNION?](#what-is-the-difference-between-join-and-union)

[What is collation?](#what-is-collation)

[Describe the difference between truncate and delete](#describe-the-difference-between-truncate-and-delete)

[How does B-trees index work?](#how-does-b-trees-index-work)

[What are statistics?](#what-are-statistics)

[How deadlock is resolved?](#how-deadlock-is-resolved)

[What is the difference among UNION, MINUS and INTERSECT?](#what-is-the-difference-among-union-minus-and-intersect)

[What is a filegroup?](#what-is-a-filegroup)

[How can I do an UPDATE statement with JOIN in SQL?](#how-can-i-do-an-update-statement-with-join-in-sql)

[How does truncate and delete operation effect Identity?](#how-does-truncate-and-delete-operation-effect-identity)

[Explain a usage difference between user defined functions and stored procedures](#explain-a-usage-difference-between-user-defined-functions-and-stored-procedures)

[What is a linked server?](#what-is-a-linked-server)

[How can we transpose a table using SQL (changing rows to column or vice-versa) ?](#how-can-we-transpose-a-table-using-sql-changing-rows-to-column-or-vice-versa-)

[What would happen without an index?](#what-would-happen-without-an-index)

[Name types of Triggers](#name-types-of-triggers)

[What are DMV's and DMF's?](#what-are-dmvs-and-dmfs)

[What's the difference between a primary key and a unique key?](#whats-the-difference-between-a-primary-key-and-a-unique-key)

[Delete duplicate values in a SQL table](#delete-duplicate-values-in-a-sql-table)

[What is the cost of having a database index?](#what-is-the-cost-of-having-a-database-index)

[How to generate row number in SQL Without ROWNUM](#how-to-generate-row-number-in-sql-without-rownum)

[Explain the difference between exclusive lock and update lock](#explain-the-difference-between-exclusive-lock-and-update-lock)

[Insert results of a stored procedure into a temporary table](#insert-results-of-a-stored-procedure-into-a-temporary-table)

[What are some other types of indexes?](#what-are-some-other-types-of-indexes)

[Name some disadvantages of a hash index](#name-some-disadvantages-of-a-hash-index)

[How does database indexing work?](#how-does-database-indexing-work)

[How does primary key constraint and unique key constraint effect null?](#how-does-primary-key-constraint-and-unique-key-constraint-effect-null)

[Select first row in each GROUP BY group (greatest-n-per-group problem)?](#select-first-row-in-each-group-by-group-greatest-n-per-group-problem)

[What is Optimistic Locking and Pessimistic locking?](#what-is-optimistic-locking-and-pessimistic-locking)



### What is PRIMARY KEY?

A **PRIMARY KEY** constraint is a unique identifier for a row within a database table. Every table should have a primary key constraint to uniquely identify each row and only one primary key constraint can be created for each table. The primary key constraints are used to enforce entity integrity.

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### Define a temp table 

In a nutshell, a temp table is a temporary storage structure. What does that mean? Basically, you can use a temp table to store data temporarily so you can manipulate and change it before it reaches its destination format.

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### What is a view?

A **view** is simply a virtual table that is made up of elements of multiple physical or “real” tables. Views are most commonly used to join multiple tables together, or control access to any tables existing in background server processes.	

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### What’s the difference between a local  temp table and a global temp table? 

* **Local tables** are accessible to a current user connected to the server. These tables disappear once the user has disconnected from the server. 
* **Global temp** tables, on the other hand, are available to all users regardless of the connection. These tables stay active until all the global connections are closed.

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### What is blocking?

SQL Server blocking occurs when one connection holds a lock on a record and other connection tries to fetch the record or update the record.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### What is the difference between WHERE clause and HAVING clause?

- WHERE clause can only be applied on a static non-aggregated column 
- we will need to use HAVING for aggregated columns.

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### What is FOREIGN KEY?

A **FOREIGN KEY** constraint prevents any actions that would destroy links between tables with the corresponding data values. A foreign key in one table points to a primary key in another table. Foreign keys prevent actions that would leave rows with foreign key values when there are no primary keys with that value. The foreign key constraints are used to enforce referential integrity.

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### What is Normalization?

It is the process of eliminating redundant data and maintaining data dependencies.

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### How can a column with a default value be added to an existing table?

Consider:
```sql
ALTER TABLE SomeTable
        ADD SomeCol Bit NULL --Or NOT NULL.
 CONSTRAINT D_SomeTable_SomeCol --When Omitted a Default-Constraint Name is autogenerated.
    DEFAULT (0)--Optional Default-Constraint.
WITH VALUES --Add if Column is Nullable and you want the Default Value for Existing Records.
```
Keep in mind that if the column is nullable, then null will be the value used for existing rows. 

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### What is DEFAULT?

**Default** allows to add values to the column if the value of that column is not set. Default can be defined on number and datetime fields. They cannot be defined on timestamp and IDENTITY columns.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### What is the difference between inner and outer join?

- Inner join returns rows when there is at least one match in both tables
- Outer join will return matching rows from both tables as well as any unmatched rows from one or both the tables 

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### Discuss INNER JOIN ON vs WHERE clause

`INNER JOIN` is ANSI syntax which you should use. INNER JOIN helps human readability, and that's a top priority. It can also be easily replaced with an OUTER JOIN whenever a need arises.

Implicit joins (with multiple `FROM` tables) become much much more confusing, hard to read, and hard to maintain once you need to start adding more tables to your query. 

###### Source

* https://stackoverflow.com/questions/3800551/select-first-row-in-each-group-by-group

[[↑] Back to top](#SQL)
### What are the difference between clustered and a non-clustered index?

* A **clustered index** is a special type of index that reorders the way records in the table are physically stored. Therefore table can have only one clustered index. The leaf nodes of a clustered index contain the data pages.
	
* A **non clustered index** is a special type of index in which the logical order of the index does not match the physical stored order of the rows on disk. The leaf node of a non clustered index does not consist of the data pages. Instead, the leaf nodes contain index rows.

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### How do I perform an IF…THEN in an SQL SELECT?

The CASE statement is the closest to IF in SQL and is supported on all versions of SQL Server:
```sql
SELECT CAST( 
   CASE
      WHEN
         Obsolete = 'N' 
         or InStock = 'Y' 
      THEN 1 
      ELSE 0 
   END AS bit) as Saleable, * 
FROM
   Product
```

###### Source

* https://stackoverflow.com/questions/63447/how-do-i-perform-an-if-then-in-an-sql-select

[[↑] Back to top](#SQL)
### Finding duplicate values in a SQL table

Simply group on both of the columns:
```sql
SELECT
    name, email, COUNT(*) as CountOf
FROM
    users
GROUP BY
    name, email
HAVING 
    COUNT(*) > 1
```

###### Source

* https://stackoverflow.com/questions/2594829/finding-duplicate-values-in-a-sql-table

[[↑] Back to top](#SQL)
### How does a hash table index work?

The reason hash indexes are used is because hash tables are extremely efficient when it comes to just looking up values. So, queries that compare for equality to a string can retrieve values very fast if they use a hash index.

For instance, the query in the question could benefit from a hash index created on the `Employee_Name` column. The way a hash index would work is that the column value will be the key into the hash table and the actual value mapped to that key would just be a pointer to the row data in the table. Since a hash table is basically an associative array, a typical entry would look something like “Abc => 0x28939″, where 0x28939 is a reference to the table row where Abc is stored in memory. Looking up a value like “Abc” in a hash table index and getting back a reference to the row in memory is obviously a lot faster than scanning the table to find all the rows with a value of “Abc” in the `Employee_Name` column.

###### Source

* https://stackoverflow.com/questions/1108/how-does-database-indexing-work

[[↑] Back to top](#SQL)
### What are the advantages of using Stored Procedures?

* Stored procedure can reduced network traffic and latency, boosting application performance.
* Stored procedure execution plans can be reused, staying cached in SQL Server's memory, reducing server overhead.
* Stored procedures help promote code reuse.
* Stored procedures can encapsulate logic. You can change stored procedure code without affecting clients.
* Stored procedures provide better security to your data.	
	

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### What is Denormalization?

It is the process of improving the performance of the database by _adding_ redundant data.

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### How to select first 5 records from a table?

```sql
-- SQL Server
SELECT TOP 5 * FROM EMP;
```
```sql
-- Oracle
SELECT * FROM EMP WHERE ROWNUM <= 5;
```

```sql
-- Generic
SELECT  name  FROM EMPLOYEE o
			   WHERE (SELECT count(*) FROM EMPLOYEE i WHERE i.name < o.name) < 5
```

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### Define ACID Properties

* **Atomicity**: It ensures all-or-none rule for database modifications.
* **Consistency**: Data values are consistent across the database.
* **Isolation**: Two transactions are said to be independent of one another.
* **Durability**: Data is not lost even at the time of server failure.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### How a database index can help performance?

The whole point of having an index is to speed up search queries by essentially cutting down the number of records/rows in a table that need to be examined. An index is a data structure (most commonly a B- tree) that stores the values for a specific column in a table.

###### Source

* https://stackoverflow.com/questions/1108/how-does-database-indexing-work

[[↑] Back to top](#SQL)
### What is the difference between UNION and UNION ALL?	

- UNION operation returns only the unique records from the resulting data set  
- UNION ALL will return all the rows, even if one or more rows are duplicated to each other.

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### What is a cursor how does it work?

**Cursor** is a database object used to manipulate data in row-by-row basis. Steps involved: 
* Declare a cursor
* Open a cursor
* Fetch row from the cursor
* Process the row fetched
* Close the cursor
* Deallocate the cursor.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### How do I UPDATE from a SELECT in SQL Server?

```sql
UPDATE
    Table_A
SET
    Table_A.col1 = Table_B.col1,
    Table_A.col2 = Table_B.col2
FROM
    Some_Table AS Table_A
    INNER JOIN Other_Table AS Table_B
        ON Table_A.id = Table_B.id
WHERE
    Table_A.col3 = 'cool'
```
or using `MERGE`:
```sql
MERGE INTO YourTable T
   USING other_table S 
      ON T.id = S.id
         AND S.tsql = 'cool'
WHEN MATCHED THEN
   UPDATE 
      SET col1 = S.col1, 
          col2 = S.col2;
```

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### What is the difference between “INNER JOIN” and “OUTER JOIN”?

Assuming you're joining on columns with no duplicates, which is a very common case:

* An **inner join** of A and B gives the result of A intersect B, i.e. the inner part of a Venn diagram intersection.
* An **outer join** of A and B gives the results of A union B, i.e. the outer parts of a Venn diagram union.
* A **left outer join** will give all rows in A, plus any common rows in B.
* A **right outer join** will give all rows in B, plus any common rows in A.
* A **full outer join** will give you the union of A and B, i.e. all the rows in A and all the rows in B. If something in A doesn't have a corresponding datum in B, then the B portion is null, and vice versa.



<div class="text-center"/>
<img src="https://i.stack.imgur.com/1UKp7.png" class="img-fluid"/>
</div>


###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### Is table size reduced, when you delete data from the table?

No the table size is not reduced, indeed the sql server marks those rows as free rows. Once you insert the new data, the free rows will get updated and then the size of the table is changed based on the data insertion. If the data is not inserted, then after a while, the rows are eliminated.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### Explain Function vs. Stored Procedure in SQL Server

The difference between SP and UDF is listed below:

```sh
+---------------------------------+----------------------------------------+
| Stored Procedure (SP)           | Function (UDF - User Defined           |
|                                 | Function)                              |
+---------------------------------+----------------------------------------+
| SP can return zero , single or  | Function must return a single value    |
| multiple values.                | (which may be a scalar or a table).    |
+---------------------------------+----------------------------------------+
| We can use transaction in SP.   | We can't use transaction in UDF.       |
+---------------------------------+----------------------------------------+
| SP can have input/output        | Only input parameter.                  |
| parameter.                      |                                        |
+---------------------------------+----------------------------------------+
| We can call function from SP.   | We can't call SP from function.        |
+---------------------------------+----------------------------------------+
| We can't use SP in SELECT/      | We can use UDF in SELECT/ WHERE/       |
| WHERE/ HAVING statement.        | HAVING statement.                      |
+---------------------------------+----------------------------------------+
| We can use exception handling   | We can't use Try-Catch block in UDF.   |
| using Try-Catch block in SP.    |                                        |
+---------------------------------+----------------------------------------+
```

###### Source

* https://stackoverflow.com/questions/1179758/function-vs-stored-procedure-in-sql-server

[[↑] Back to top](#SQL)
### What are row constructors?

**ROW Constructor** or **Table Value Constructor** means to create a row set by using the `VALUES()` clause. This allows multiple rows of data to be specified in a single DML statement.

```sql
SELECT * 
FROM (
VALUES
    (1, 'cust 1', '(111) 111-1111', 'address 1'),
    (2, 'cust 2', '(222) 222-2222', 'address 2'),
    (3, 'cust 3', '(333) 333-3333', 'address 3'),
    (4, 'cust 4', '(444) 444-4444', 'address 4'),
    (5, 'cust 5', '(555) 555-5555', 'address 5')
) AS C (CustID, CustName, phone, addr);

```

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### What is the difference between JOIN and UNION?

- SQL JOIN allows us to “lookup” records on other table based on the given conditions between two tables. 
- UNION operation allows us to add 2 similar data sets to create resulting data set that contains all the data from the source data sets. Union does not require any condition for joining.

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### What is collation?

**Collation** defines a set of rules that determines how data is sorted and compared. Once the collation has been defined, you cannot change the collation rules until you re-create it or drop the entity.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### Describe the difference between truncate and delete 

* **Delete** command removes the rows from a table based on the condition that we provide with a WHERE clause. 

* **Truncate** will actually remove all the rows from a table and there will be no data in the table after we run the truncate command.

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### How does B-trees index work?

The reason **B- trees** are the most popular data structure for indexes is due to the fact that they are time efficient – because look-ups, deletions, and insertions can all be done in _logarithmic time_. And, another major reason B- trees are more commonly used is because the data that is stored inside the B- tree can be sorted. The RDBMS typically determines which data structure is actually used for an index. But, in some scenarios with certain RDBMS’s, you can actually specify which data structure you want your database to use when you create the index itself.

###### Source

* https://stackoverflow.com/questions/1108/how-does-database-indexing-work

[[↑] Back to top](#SQL)
### What are statistics?

**Statistics** define how well a query can be executed with low resource consumption.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### How deadlock is resolved?

Deadlock is automatically resolved by SQL Server. It identifies the process which has less overhead and accordingly it rollbacks the transaction associated with that process.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### What is the difference among UNION, MINUS and INTERSECT?

- UNION combines the results from 2 tables and eliminates duplicate records from the result set.
- MINUS operator when used between 2 tables, gives us all the rows from the first table except the rows which are present in the second table.
- INTERSECT operator returns us only the matching or common rows between 2 result sets.

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### What is a filegroup?

**Filegroup** is a collection of datafiles which are managed as a single unit. You can have one primary filegroup per database and many user defined filegroups. Log files cannot be part of a filegroup due to difference in structure.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### How can I do an UPDATE statement with JOIN in SQL?

```sql
update u
set u.assid = s.assid
from ud u
    inner join sale s on
        u.id = s.udid
```
Without `JOIN`:
```sql
update ud 
set assid = sale.assid
from sale
where sale.udid = id
```


###### Source

* https://stackoverflow.com/questions/1293330/how-can-i-do-an-update-statement-with-join-in-sql

[[↑] Back to top](#SQL)
### How does truncate and delete operation effect Identity?

Truncate _resets_ the Identity to its base value where as _delete_ does not reset it to the base value.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### Explain a usage difference between user defined functions and stored procedures

**User defined functions** can be used anywhere in the queries i.e. within where/having/select section where as stored procedures can't. 

**Note:** Stored procedures can be used with insert statements. UDFs can also be used in join operations and UDFs can be used to return tables which can be joined with other tables.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### What is a linked server?

**Linked server** facilitates the ease of linking with heterogeneous servers. Using linked servers, you can manipulate data on the remote servers and even integrate with local data. 

Stored procedures: `sp_linkedservers` gives you the list of linked servers available on the server.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### How can we transpose a table using SQL (changing rows to column or vice-versa) ?

The usual way to do it in SQL is to use CASE statement or DECODE statement

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### What would happen without an index?

Database software would literally have to look at every single row in the `Employee` table to see if the `Employee_Name` for that row is ‘Abc’. And, because we want every row with the name ‘Abc’ inside it, we can not just stop looking once we find just one row with the name ‘Abc’, because there could be other rows with the name Abc. So, every row up until the last row must be searched – which means thousands of rows in this scenario will have to be examined by the database to find the rows with the name ‘Abc’. This is what is called a **full table scan**.

###### Source

* https://stackoverflow.com/questions/1108/how-does-database-indexing-work

[[↑] Back to top](#SQL)
### Name types of Triggers

They are three different types of triggers:
   1. **DML Triggers**: These are of two kinds:
   	 * _Instead of Triggers_: These are invoked in place of the triggering action such as insert, update or delete.
        * _After Triggers_: These are invoked after the triggering action such as insert, update or delete.
   2. **DDL Triggers**: These are invoked against DDL statements. These are always _After Triggers_.
   3. **Logon Triggers**: These are invoked when a Logon event occurs and before the user session is established.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### What are DMV's and DMF's?

**Data management views** and **data management functions** provide information about the state of sql server in other words they are responsible for providing information about health of the sql server.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### What's the difference between a primary key and a unique key?

Both primary key and unique key enforces uniqueness of the column on which they are defined. 

But by default primary key creates a _clustered index_ on the column, where are unique creates a _non-clustered_ index by default. 

Another major difference is that, _primary key doesn't allow NULLs, but unique key allows one NULL only_.	

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### Delete duplicate values in a SQL table

Consider:
```sql
DELETE FROM users
WHERE id IN (
    SELECT id/*, name, email*/
    FROM users u, users u2
    WHERE u.name = u2.name AND u.email = u2.email AND u.id > u2.id
)
```
Or using `PARTITION BY`:
```sql
DELETE d
    FROM @YourTable d
        INNER JOIN (SELECT
                        y.id,y.name,y.email,ROW_NUMBER() OVER(PARTITION BY y.name,y.email ORDER BY y.name,y.email,y.id) AS RowRank
                        FROM @YourTable y
                            INNER JOIN (SELECT
                                            name,email, COUNT(*) AS CountOf
                                            FROM @YourTable
                                            GROUP BY name,email
                                            HAVING COUNT(*)>1
                                        ) dt ON y.name=dt.name AND y.email=dt.email
                   ) dt2 ON d.id=dt2.id
        WHERE dt2.RowRank!=1
SELECT * FROM @YourTable
```

###### Source

* https://stackoverflow.com/questions/2594829/finding-duplicate-values-in-a-sql-table

[[↑] Back to top](#SQL)
### What is the cost of having a database index?

It takes up space – and the larger your table, the larger your index. Another performance hit with indexes is the fact that whenever you add, delete, or update rows in the corresponding table, the same operations will have to be done to your index. Remember that an index needs to contain the same up to the minute data as whatever is in the table column(s) that the index covers.

As a general rule, an index should only be created on a table if the data in the indexed column will be queried frequently.

###### Source

* https://stackoverflow.com/questions/1108/how-does-database-indexing-work

[[↑] Back to top](#SQL)
### How to generate row number in SQL Without ROWNUM

Consider:
```sql
SELECT name, sal, (SELECT COUNT(*)  FROM EMPLOYEE i WHERE o.name >= i.name) row_num
		FROM EMPLOYEE o 
		order by row_num
```

###### Source

* https://github.com/dhaval1406/SQL

[[↑] Back to top](#SQL)
### Explain the difference between exclusive lock and update lock

* In case of **exclusive lock**, no other lock can be acquired on that row or table. Every process has to wait until the process which holds the lock releases it.

* In case of **update lock**, while reading the row or a record, you can have any other lock associated with that row or record. In case of updating the record, update lock changes itself to exclusive lock and no other process can obtain a lock on that row until the lock is released.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### Insert results of a stored procedure into a temporary table

You can use OPENROWSET for this. I've also included the sp_configure code to enable Ad Hoc Distributed Queries, in case it isn't already enabled.

```sql
CREATE PROC getBusinessLineHistory
AS
BEGIN
    SELECT * FROM sys.databases
END
GO

sp_configure 'Show Advanced Options', 1
GO
RECONFIGURE
GO
sp_configure 'Ad Hoc Distributed Queries', 1
GO
RECONFIGURE
GO

SELECT * INTO #MyTempTable FROM OPENROWSET('SQLNCLI', 'Server=(local)\SQL2008;Trusted_Connection=yes;',
     'EXEC getBusinessLineHistory')

SELECT * FROM #MyTempTable
```

###### Source

* https://stackoverflow.com/questions/653714/insert-results-of-a-stored-procedure-into-a-temporary-table

[[↑] Back to top](#SQL)
### What are some other types of indexes?

Indexes that use a **R-tree** data structure are commonly used to help with _spatial_ problems. For instance, a query like “Find all of the Starbucks within 2 kilometers of me” would be the type of query that could show enhanced performance if the database table uses a R- tree index.

Another type of index is a **bitmap index**, which work well on columns that contain Boolean values (like true and false), but many instances of those values – basically columns with low selectivity.

###### Source

* https://www.programmerinterview.com/index.php/database-sql/what-is-an-index/

[[↑] Back to top](#SQL)
### Name some disadvantages of a hash index

Hash tables are not sorted data structures, and there are many types of queries which hash indexes can not even help with. For instance, suppose you want to find out all of the employees who are less than 40 years old. How could you do that with a hash table index? Well, it’s not possible because a hash table is only good for looking up key value pairs – which means queries that check just for _equality_.

###### Source

* https://stackoverflow.com/questions/1108/how-does-database-indexing-work

[[↑] Back to top](#SQL)
### How does database indexing work?

**Indexing** is a way of sorting a number of records on multiple fields. Creating an index on a field in a table creates another data structure (stored on the disc) which holds the field value, and a pointer to the record it relates to. This index structure is then sorted, allowing Binary Searches to be performed on it, which has log2 N block accesses. Also since the data is sorted given a non-key field, the rest of the table doesn’t need to be searched for duplicate values, once a higher value is found.

The whole point of having an index is to speed up search queries by essentially cutting down the number of records/rows in a table that need to be examined. An index is a data structure (most commonly a B- tree or hash table) that stores the values for a specific column in a table.

Given the nature of a binary search, the **cardinality or uniqueness** of the data is important. Indexing on a field with a cardinality of 2 would split the data in half, whereas a cardinality of 1,000 would return approximately 1,000 records. 

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### How does primary key constraint and unique key constraint effect null?

Primary key constraints allow no null values in the specified column where as unique key constraint allows a single null value not multiple null values.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
### Select first row in each GROUP BY group (greatest-n-per-group problem)?

Consider:
```sql
WITH summary AS (
    SELECT p.id, 
           p.customer, 
           p.total, 
           ROW_NUMBER() OVER(PARTITION BY p.customer 
                                 ORDER BY p.total DESC) AS rk
      FROM PURCHASES p)
SELECT s.*
  FROM summary s
 WHERE s.rk = 1
```

###### Source

* https://stackoverflow.com/questions/3800551/select-first-row-in-each-group-by-group

[[↑] Back to top](#SQL)
### What is Optimistic Locking and Pessimistic locking?

**Optimistic Locking** is a strategy where you read a record, take note of a version number (other methods to do this involve dates, timestamps or checksums/hashes) and check that the version hasn't changed before you write the record back. When you write the record back you filter the update on the version to make sure it's atomic. (i.e. hasn't been updated between when you check the version and write the record to the disk) and update the version in one hit.

If the record is dirty (i.e. different version to yours) you abort the transaction and the user can re-start it.

This strategy is most applicable to high-volume systems and three-tier architectures where you do not necessarily maintain a connection to the database for your session. In this situation the client cannot actually maintain database locks as the connections are taken from a pool and you may not be using the same connection from one access to the next.

**Pessimistic Locking** is when you lock the record for your exclusive use until you have finished with it. It has much better integrity than optimistic locking but requires you to be careful with your application design to avoid Deadlocks. To use pessimistic locking you need either a direct connection to the database (as would typically be the case in a two tier client server application) or an externally available transaction ID that can be used independently of the connection.

The disadvantage of pessimistic locking is that a resource is locked from the time it is first accessed in a transaction until the transaction is finished, making it inaccessible to other transactions during that time.

###### Source

* https://github.com/chetansomani/SQL-Interview-Questions

[[↑] Back to top](#SQL)
