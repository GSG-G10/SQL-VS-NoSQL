
## Introduction
At the beginning, the acronym itself describes what both of terms react.
  For SQL databases (Structured Query Language) that means we care more about the relations between data, SQL databases have a predefined schema and it is the perfect choice for the complex query intensive environment.

  Otherwise NOSQL databases (Not Only Structured Query Language) that means we care more about the rapidity of data than correct data, NoSQL databases use dynamic schema for unstructured data.![](https://i.imgur.com/52Ckcxn.png)
  
![](https://i.imgur.com/Vpa105o.png)



---
### What is SQL?
SQL, short for Structured Query Language, is a programming language that is used to manage data in relational databases. Relational databases use relations (typically called tables) to store data and then match that data by using common characteristics within the dataset.

**Some popular SQL database systems include:**

* Oracle
* Microsoft SQL Server
* PostgreSQL
* MySQL
* MariaDB
 
 ##### SQL Databases (Relational)
SQL is short for Structured Query Language, basically meaning a very firm way of sorting through data in the form of tables, columns, and rows. How is data structured in an SQL database? The table itself would be made up really of one variable or object that we would be looking through. The column would represent the data point itself that needs to be stored and the row is a record of the data points per column.![](https://i.imgur.com/0fqqU9g.png)
![](https://i.imgur.com/orvLkMw.png)


### What is NoSQL?
A NoSQL database, on the other hand, is self-describing, so does not require a schema. Nor does it enforce relations between tables in all cases. All its documents are JSON documents, which are complete entities that one can readily read and understand.

**Some popular NoSQL databases include:**

* MongoDB
* Google Cloud Firestore
* Cassandra
* Redis
* Apache HBase
* Amazon DynamoDB



#### NoSQL Databases (Non-Relational)
In contrast to a relational database, a NoSQL database is one that is less structured/confined in format, and thus, allows for more flexibility and adaptability. If you are going to be dealing with a dataset that isn’t clearly defined, meaning not organized or structured, you likely won’t have the luxury of establishing defined tables and relationships amongst the dataset.

## What are the Benefits of NoSQL Databases?
NoSQL databases offer many benefits over relational databases. NoSQL databases have flexible data models, scale horizontally, have incredibly fast queries, and are easy for developers to work with.

* **Flexible data models**

NoSQL databases typically have very flexible schemas. A flexible schema allows you to easily make changes to your database as requirements change. You can iterate quickly and continuously integrate new application features to provide value to your users faster.

* **Horizontal scaling**

Most SQL databases require you to scale-up vertically (migrate to a larger, more expensive server) when you exceed the capacity requirements of your current server. Conversely, most NoSQL databases allow you to scale-out horizontally, meaning you can add cheaper, commodity servers whenever you need to.
- NoSQL
![](https://i.imgur.com/gTpFcQN.png)
- VS SQL
![](https://i.imgur.com/h4UY3C8.png)



* **Fast queries**

Queries in NoSQL databases can be faster than SQL databases. Why? Data in SQL databases is typically normalized, so queries for a single object or entity require you to join data from multiple tables. As your tables grow in size, the joins can become expensive. However, data in NoSQL databases is typically stored in a way that is optimized for queries. The rule of thumb when you use MongoDB is Data is that is accessed together should be stored together. Queries typically do not require joins, so the queries are very fast.

* **Easy for developers**

Some NoSQL databases like MongoDB map their data structures to those of popular programming languages. This mapping allows developers to store their data in the same way that they use it in their application code. While it may seem like a trivial advantage, this mapping can allow developers to write less code, leading to faster development time and fewer bugs.


### Making the decision
Choosing a database depends majorly on the type of data and its agility that your project needs to store.

  How to choose your database structure type? The answer can easily be found. If the project is expected to see little changes, needs to handle huge and versatile amount of data, or the database entities and schema is ambiguous at the start, go for NoSQL you can use MongoDB as an example.

  However, if the project needs to handle small and homogeneous data, and the databases entities are clearly defined with unambiguous and many relationships which rarely is the case especially when we talk about big data, SQL is a good fit you can use MYSQL or oracle as examples.![](https://i.imgur.com/Yofq5bJ.png)



---

| Attempt |  SQL Databases |  NoSQL Databases |
| :---:   | :-: | :-: |
| Data Storage Model | Tables with fixed rows and columns | Document: JSON documents, Key-value: key-value pairs, Wide-column: tables with rows and dynamic columns, Graph: nodes and edges|
|Development History| Developed in the 1970s with a focus on reducing data duplication | Developed in the late 2000s with a focus on scaling and allowing for rapid application change driven by agile and DevOps practices. |
| Examples | Oracle, MySQL, Microsoft SQL Server, and PostgreSQL | Document: MongoDB and CouchDB, Key-value: Redis and DynamoDB, Wide-column: Cassandra and HBase, Graph: Neo4j and Amazon Neptune |
| Primary Purpose | General purpose | Document: general purpose, Key-value: large amounts of data with simple lookup queries, Wide-column: large amounts of data with predictable query patterns, Graph: analyzing and traversing relationships between connected data |
| Schemas | Rigid | Flexible |
| Scaling | Vertical (scale-up with a larger server) | Horizontal (scale-out across commodity servers) |
| Joins | Typically requiredJoins | Typically not requiredJoins |
| Data to Object Mapping | Requires ORM (object-relational mapping) | Many do not require ORMs. MongoDB documents map directly to data structures in most popular programming languages. |


## Conclusion
In summary, the five key differences between SQL vs. NoSQL are:

1. SQL databases are **relational**, NoSQL databases are **non-relational**.
2. SQL databases use structured query language and have a predefined schema. NoSQL databases have dynamic schemas for unstructured data.
3. SQL databases are **vertically** scalable, while NoSQL databases are **horizontally** scalable.
4. SQL databases are ***table-based***, while NoSQL databases are document, key-value, graph, or wide-column stores.
5. SQL databases are better for multi-row transactions, while NoSQL is better for unstructured data like documents or JSON.