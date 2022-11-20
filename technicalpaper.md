# SQL CONCEPTS

## ACID:
Definition: ACID stands for atomicity, consistency, isolation, and durability. Together, these ACID properties ensure that a set of database operations grouped together in a transaction leave the database in a valid state even in the event of unexpected errors.
- Atomicity: A transaction must be Atomic, that means all changes made by the transaction are completed as a single unit, or none of the changes are made. If a partial transaction were committed, the atomic property is violated, and the database is left in an inconsistent state.
- Consistency: Consistency in database systems refers to the requirement that any given database transaction must change affected data only in allowed ways. For a database to be consistent, data written to the database must be valid according to all defined rules, including constraints, cascades, triggers, or any combination.
- Isolation: Isolation is the separation of resource or data modifications made by different transactions. Isolation levels are described for which concurrency side effects are allowed.
- Durability: Durability ensures that changes made to the database transactions that are successfully committed will survive permanently, even in the case of system failures. This ensures that the data within the database will not be corrupted by Service outages, Crashes.

## CAP THEOREM:
The CAP theorem states that it is not possible to guarantee all three of the desirable properties – consistency, availability, and partition tolerance at the same time in a distributed system with data replication.
- Consistency: Consistency means that the nodes will have the same copies of a replicated data item visible for various transactions. A guarantee that every node in a distributed cluster returns the same, most recent and a successful write. Consistency refers to every client having the same view of the data.
- Availability: Availability means that each read or write request for a data item will either be processed successfully or will receive a message that the operation cannot be completed. Every non-failing node returns a response for all the read and write requests in a reasonable amount of time.
- Partition Tolerance: Partition tolerance means that the system can continue operating even if the network connecting the nodes has a fault that results in two or more partitions, where the nodes in each partition can only communicate among each other. That means, the system continues to function and upholds its consistency guarantees in spite of network partitions. 

## JOINS:
A join clause is used to combine rows from two or more tables, based on a related column between them.
1. Types of Joins:
- INNER JOIN: This join returns those records which have matching values in both the tables. Syntax: SELECT column, another column FROM mytable INNER JOIN another_table ON mytable.id = anothertable.ID;
- LEFT OUTER JOIN: This join returns records from the left table, and also those records which satisfy the condition from the right table. Syntax: SELECT column, another column FROM mytable LEFT OUTER JOIN another_table ON mytable.id = anothertable.ID;
- RIGHT OUTER JOIN: This join returns records from the right table, and also those records which satisfy the condition from the left table. Syntax: SELECT column, another column FROM mytable RIGHT OUTER JOIN another_table ON mytable.id = anothertable.ID;
- FULL OUTER JOIN: This join returns all those records which either have a match in the left or the right table. Syntax: SELECT column, another column FROM mytable FULL OUTER JOIN another_table ON mytable.id = anothertable.ID;

## Aggregations:
In database management an aggregate function is a function where the values of multiple rows are grouped together as input on certain criteria to form a single value of more significant meaning.
1. Various aggregate Functions
- Count()
- Sum()
- Avg()
- Min()
- Max()

## Normalization:
It is the process of organizing data in a database. This includes creating tables and establishing relationships between those tables according to rules designed both to secure the data and to make the database more flexible by removing duplicates and inconsistent dependency.
1. Forms of Normalization and their rules :
- First normal form(1NF) — First normal form (1NF) The type of entity is 1NF because it does not contain repeated data groups.
- Second normal form(2NF) — Second Normal Form (2NF) The type of entity is in 2NF when it is in 1NF and when all of its non-key attributes are entirely dependent on its primary key.
- Third normal form(3NF) — Third normal form (3NF) The type of an object is 3NF when it is 2NF and all its attributes depend directly on the primary key.
2. Advantages of Normalization of data:
- Further Storage: As databases fill up with data, redundant categorization and elimination make space for gigabytes and terabytes, which will be needed. The processing efficiency decreases when a device is filled with unnecessary material. Your devices can work faster and load faster after cleaning digital memory, ensuring data processing is performed at a more effective pace.
- Faster Solution: Speaking of faster procedures, you can arrange your data without the need to adjust further after normalization becomes a simple task. Instead of attempting to convert insane data that has not been properly processed, this lets different departments inside an organization save valuable time.
- Accurate Segmentation: Groups can be easily divided into categories based on names and occupations as everything is segmented properly by using data normalization.

## Indexes:
An index is a schema object. It is used by the server to speed up the retrieval of rows by using a pointer. It can reduce disk input or output by using a rapid path access method to locate data quickly. An index helps to speed up select queries and where clauses, but it slows down data input, with the update and the insert statements. Indexes can be created or dropped with no effect on the data. 

##Transactions:
Transactions group a set of tasks into a single execution unit. Each transaction begins with a specific task and ends when all the tasks in the group successfully complete. If any of the tasks fail, the transaction fails. Therefore, a transaction has only two results: success or failure.  It is important to note that these statements cannot be used while creating tables and are only used with the DML Commands such as  insert, delete and update.

## Locking Mechanism:
Locking mechanisms are a way for databases to produce sequential data output without the sequential steps. The locks provide a method for securing the data that is being used so no irrgeularities can occur like lost data or additional data that can be added because of the loss of a transaction. 

## Database isolation levels:

## Triggers:
A trigger is a stored procedure in database which automatically invokes whenever a special event in the database occurs. For example, a trigger can be invoked when a row is inserted into a specified table or when certain table columns are being updated. 
