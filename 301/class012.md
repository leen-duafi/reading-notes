|       SQL   |        	NoSQL         |
| ----------- | --------------------- |
|SQL databases are primarily called as Relational Databases|NoSQL database are primarily called as non-relational or distributed database.  |
|SQL databases have predefined schema | NoSQL databases have dynamic schema for unstructured data.   |
|QL database examples: MySql, Oracle, Sqlite, Postgres and MS-SQL |NoSQL database examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb     |
|SQL databases emphasizes on ACID properties ( Atomicity, Consistency, Isolation and Durability)|NoSQL database follows the Brewers CAP theorem ( Consistency, Availability and Partition tolerance )|     
|SQL databases uses SQL ( structured query language ) for defining and manipulating the data, which is very powerfu|NoSQL database, queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language). The syntax of using UnQL varies from database to database.     |

**What kind of data is a good fit for an SQL database?**

sQL databases are good fit for the complex query intensive environment

**Give a real world example.**

MySql, Oracle, Sqlite, Postgres and MS-SQL. NoSQL

**What kind of data is a good fit a NoSQL database?**

NoSQL database are highly preferred for large data set (i.e for big data). Hbase is an example for this purpose.

**Give a real world example.**

MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb

**Which type of database is best for hierarchical data storage?**

NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data. NoSQL database are highly preferred for large data set

**Which type of database is best for scalability?**

In most typical situations, SQL databases are vertically scalable. You can manage increasing load by increasing the CPU, RAM, SSD, etc, on a single server. On the other hand, NoSQL databases are horizontally scalable. You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffie



















**What does SQL stand for?**

stands for Structured Query Language

**What is a realational database?**

A relational database is a type of database that stores and provides access to data points that are related to one another. Relational databases are based on the relational model, an intuitive, straightforward way of representing data in tables. In a relational database, each row in the table is a record with a unique ID called the key. The columns of the table hold attributes of the data, and each record usually has a value for each attribute, making it easy to establish the relationships among data points

**What type of structure does a relational database work with?**

A traditional and widely-used data structure is called "B-tree." B-tree structures are a standard part of computer science textbooks and are used in most (if not all) RDBMS products.

**What is a ‘schema’?**

A database schema represents the logical configuration of all or part of a relational database. It can exist both as a visual representation and as a set of formulas known as integrity constraints that govern a database. These formulas are expressed in a data definition language, such as SQL

a database schema indicates how the entities that make up the database relate to one another, including tables, views, stored procedures, and more.

**the schema for a NoSQL database** is flexible, meaning there is no fixed structure to the data, data types and lengths for data elements. Data can be stored in a free-form, or schemaless manner. This approach offers programmers a higher degree of flexibility, which can ease development efforts.

**What is a NoSQL database?**

non tabular, and store data differently than relational tables. NoSQL databases come in a variety of types based on their data model. The main types are document, key-value, wide-column, and graph. They provide flexible schemas and scale easily with large amounts of data and high user loads.

**Howo does it work?**

Each of the systems labelled with the generic name works differently, but the basic idea is to offer better scalability and performance by using DB models that don't support all the functionality of a generic RDBMS, but still enough functionality to be useful. In a way it's like MySQL, which at one time lacked support for transactions but, exactly because of that, managed to outperform other DB systems. 

**What is inside of a Mongo database?**

MongoDB stores data records as documents (specifically BSON documents) which are gathered together in collections. A database stores one or more collections of documents.

***Which is more flexible - SQL or MongoDB? and why.**

 MongoDB is more flexible and ensures high and diverse data availability

**What is the disadvantage of a NoSQL database?**

* NoSQL databases don’t have the reliability functions which Relational Databases have (basically don’t support ACID).
* In order to support ACID developers will have to implement their own code, making their systems more complex.
* NoSQL is not compatible (at all) with SQL
* NoSQL are very new compared to Relational Databases, which means that are far less stable and may have a lot less functionalities.

