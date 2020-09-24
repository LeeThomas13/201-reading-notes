# DB Normalization

[Link to Article](https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/)

This is basically how to organize a database into columns and rows. The idea is that you keep each table doing only a couple things, and the topics supporting it only refer to the main topic. By limiting a table to one purpose you reduce the number of duplicate data contained within your database. 


There are three common forms of database normalization: 1st, 2nd, and 3rd normal form. They are also abbreviated as 1NF, 2NF, and 3NF respectively. 
There are several additional forms, such as BCNF, but I consider those advanced, and not too necessary to learn in the beginning.


First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.
Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key


[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)