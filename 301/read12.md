# Read12 :Readings: Mongo and Mongoose

Fill in the chart below with five differences between SQL and NoSQL databases:


SQL databases are primarily called as Relational Databases (RDBMS); whereas NoSQL database are primarily called as non-relational or distributed database.
SQL databases are table based databases whereas NoSQL databases are document based, key-value pairs, graph databases or wide-column stores. This means that SQL databases represent data in form of tables which consists of n number of rows of data whereas NoSQL databases are the collection of key-value pair, documents, graph databases or wide-column stores which do not have standard schema definitions which it needs to adhered to.
SQL databases have predefined schema whereas NoSQL databases have dynamic schema for unstructured data.
SQL databases are vertically scalable whereas the NoSQL databases are horizontally scalable. SQL databases are scaled by increasing the horse-power of the hardware. NoSQL databases are scaled by increasing the databases servers in the pool of resources to reduce the load.
SQL databases uses SQL ( structured query language ) for defining and manipulating the data, which is very powerful. In NoSQL database, queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language). The syntax of using UnQL varies from database to database.
SQL database examples: MySql, Oracle, Sqlite, Postgres and MS-SQL. NoSQL database examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb
For complex queries: SQL databases are good fit for the complex query intensive environment whereas NoSQL databases are not good fit for complex queries. On a high-level, NoSQL don’t have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as SQL query language.

. MySQL Community Edition
MySQL database is very popular open-source database. It is generally been stacked with apache and PHP, although it can be also stacked with nginx and server side javascripting using Node js. The following are some of MySQL benefits and strengths:

Replication: By replicating MySQL database across multiple nodes the work load can be reduced heavily increasing the scalability and availability of business application
Sharding: MySQL sharding os useful when there is large no of write operations in a high traffic website. By sharding MySQL servers, the application is partitioned into multiple servers dividing the database into small chunks. As low cost servers can be deployed for this purpose, this is cost effective.
Memcached as a NoSQL API to MySQL: Memcached can be used to increase the performance of the data retrieval operations giving an advantage of NoSQL api to MySQL server.
Maturity: This database has been around for a long time and tremendous community input and testing has gone into this database making it very stable.
Wide range of Platforms and Languages: MySql is available for all major platforms like Linux, Windows, Mac, BSD and Solaris. It also has connectors to languages like Node.js, Ruby, C#, C++, C, Java, Perl, PHP and Python.
Cost effectiveness: It is open source and free.


### What kind of data is a good fit for an SQL database?
MySQL database is very popular open-source database. It is generally been stacked with apache and PHP, although it can be also stacked with nginx and server side javascripting using Node js.

### Give a real world example.
SQL database examples: MySql, Oracle, Sqlite, Postgres and MS-SQL. NoSQL

### What kind of data is a good fit a NoSQL database?
For complex queries: SQL databases are good fit for the complex query intensive environment whereas NoSQL databases are not good fit for complex queries. On a high-level, NoSQL don’t have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as SQL query language.

### Give a real world example.
For complex queries: SQL databases are good fit for the complex query intensive environment whereas NoSQL databases are not good fit for complex queries. On a high-level, NoSQL don’t have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as SQL query language.


### Which type of database is best for hierarchical data storage?
For the type of data to be stored: SQL databases are not best fit for hierarchical data storage. But, NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data. NoSQL database are highly preferred for large data set (i.e for big data). Hbase is an example for this purpose.

### Which type of database is best for scalability?
For scalability: In most typical situations, SQL databases are vertically scalable. You can manage increasing load by increasing the CPU, RAM, SSD, etc, on a single server. On the other hand, NoSQL databases are horizontally scalable. You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic.


### What does SQL stand for?
stands for Structured Query Language. SQL is used to communicate with a database. According to ANSI (American National Standards Institute), it is the standard language for relational database management systems.

### What is a realational database?

A relational database is a type of database that stores and provides access to data points that are related to one another. ... In a relational database, each row in the table is a record with a unique ID called the key.

### What type of structure does a relational database work with?

The relational model means that the logical data structures—the data tables, views, and indexes—are separate from the physical storage structures. This separation means that database administrators can manage physical data storage without affecting access to that data as a logical structure.

### What is a ‘schema’?

Schema, in social science, mental structures that an individual uses to organize knowledge and guide cognitive processes and behaviour. People use schemata (the plural of schema) to categorize objects and events based on common elements and characteristics and thus interpret and predict the world.

### What is a NoSQL database?
SQL: Relational databases
First, let’s take a look at one of the main features that separates these two systems: the way they structure data. A relational database—or, an SQL database, named for the language it’s written in, Structured Query Language (SQL)—is the more rigid, structured way of storing data, like a phone book. Developed by IBM in the 1970s, a relational database consists of two or more tables with columns and rows. Each row represents an entry, and each column sorts a very specific type of information, like a name, address, and phone number. The relationship between tables and field types is called a schema. In a relational database, the schema must be clearly defined before any information can be added.

### Howo does it work?
One way of understanding the appeal of NoSQL databases from a design perspective is to look at how the data models of a SQL and a NoSQL database might look in an oversimplified example using address data.

The SQL Case. For an SQL database, setting up a database for addresses begins with the logical construction of the format and the expectation that the records to be stored are going to remain relatively unchanged. After analyzing the expected query patterns, an SQL database might optimize storage in two tables, one for basic information and one pertaining to being a customer, with last name being the key to both tables. Each row in each table is a single customer, and each column has the following fixed attributes:

Last name :: first name :: middle initial :: address fields :: email address :: phone number
Last name :: date of birth :: account number :: customer years :: communication preferences

### What is inside of a Mongo database?
MongoDB is a source-available cross-platform document-oriented database program. Classified as a NoSQL database program, MongoDB uses JSON-like documents with optional schemas. MongoDB is developed by MongoDB Inc. and licensed under the Server Side Public License (SSPL).

### Which is more flexible - SQL or MongoDB? and why.
MySQL is a popular, free-to-use, and open-source relational database management system (RDBMS) developed by Oracle. As with other relational systems, MySQL stores data using tables and rows, enforces referential integrity and uses structured query language (SQL) for data access. When users need to retrieve data from a MySQL database, they must construct an SQL query that joins multiple tables together to create the view on the data they require.

Database schemas and data models need to be defined ahead of time, and data must match this schema to be stored in the database. This rigid approach to storing data offers some degree of safety, but trades this for flexibility. If a new type or format of data needs to be stored in the database, schema migration must occur, which can become complex and expensive as the size of the database grows.

MongoDB is also free to use and open source; however, its design principles differ from traditional relational systems. Often styled as a non-relational (or NoSQL) system, MongoDB adopts a significantly different approach to storing data, representing information as a series of JSON-like documents (actually stored as binary JSON, or BSON), as opposed to the table and row format of relational systems.

MongoDB documents consist of a series of key/value pairs of varying types, including arrays and nested documents; however, the key difference is that the structure of the key/value pairs in a given collection can vary from document to document. This more flexible approach is possible because documents are self-describing.

### What is the disadvantage of a NoSQL database?
Disadvantages
NoSQL databases don’t have the reliability functions which Relational Databases have (basically don’t support ACID).
This also means that NoSQL databases offer consistency in performance and scalability.
In order to support ACID developers will have to implement their own code, making their systems more complex.
This may reduce the number of safe applications that commit transactions, for example bank systems.