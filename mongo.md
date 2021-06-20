# Mongo and Mongoose

nosql vs sql

SQL|NoSQL
----|--------------------------------
relational databases|non-relational databases
table-based|document based, key-value pairs, graph, or wide-column
small data sets, not good for hierarchical storage |can handle large data sets, and good for hierarchical storage
good for complex queries |not good for complex queries
vertically scalable (can increase load by increasing variables such as CPU and RAM)|horizontally scalable (add more servers for handling more traffic)

**Database best for hierarchical storage**: NoSQL

**Database best for scalability**: SQL

## What kind of data is a good fit for an SQL database?
Smaller data systems with complex queries, and non-hierarchical data organization. Perhaps this could be a small amount of very layererd/interconnected information.

## What kind of data is a good fit a NoSQL database?
Larger data sets that can be stored in a JSON-like way, and don't need to handle complex queries. Perhaps this could be something like tons of weather data.

### sql vs nosql VIDEO
SQL= Structured Query Language

SQL is not a database, it is a language that lets you access data in a database

## What is a realational database? What type of structure does a relational database work with?
A relational database supports the SQL language, works with tables, which are built using schemas. These tables are often related to one another, and have data in rows of the table that are used by other tables. Information in rows can point to other items of information in other tables.

## What is a ‘schema’?
A schema is a combination of rules that determine how data is added to a database. It can have different fields like id, name, description, etc. Each new entry will have values corresponding to the schema.

## What is a NoSQL database? How does it work? What is inside of a Mongo database?
MongoDB is a NoSQL database. It follows these guidelines below.

A NoSQL database is better at storing large amounts of data. No tables, but collections of data. There are documents inside of collections, which resemble JSON. They don't have to follow strict rules of needing all the same rules of a schema- they can have different key/value pairs.

In general, no relations are found in a NoSQL. This makes it less good for managing complex queries.

One disadvantage is that NoSQL databases can lead to duplicate data.

## Which is more flexible - SQL or MongoDB? and why.
This is flexible because you can add new data with different parameters that you hadn't initially set up. If you were using SQL, you would need to go back and add data if you added a new field.