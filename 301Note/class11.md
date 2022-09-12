## Readings: Mongo and Mongoose

#### nosql vs sql

1. Fill in the chart below with five differences between SQL and NoSQL databases:
  - SQL is relational database and NoSQL is a non-relational database
  - SQL is table based data and NoSQL databases range from key-value pairs, graphs, wide-column stores
- SQL is vertically scalable and NoSQL is horizontally scalable
- SQL is for defining and manipulating data and NoSQL is for collecting documents
- SQL is best for complex queries and NoSQL is good for hierarchical data storage

2. What kind of data is a good fit for an SQL database?
Give a real world example.
  - transactional type application, more stable and promising of automicity of data 

3. What kind of data is a good fit a NoSQL database?
Give a real world example.
  - Hierarchial data storage is best fit to use NoSQL
  - Web applications using compartmental data

4. Which type of database is best for hierarchical data storage?
  - NoSql

5. Which type of database is best for scalability?
  - SQL

**Videos**
#### sql vs nosql (Video)

1. What does SQL stand for?
  - Structured query language : Language to wright database queires using key words, syntax, and data. Commands to get/push, and manipulate data.

2. What is a relational database?
  - Database that works with certain assumptions. Uses tables

3. What type of structure does a relational database work with?
  - tables: more than one table that are interrelated 
    - have feilds (columns)
    - has records (rows)
  - store data in interrelated tables of data which can be manipulated via SQL methods
4. What is a ‘schema’?
  - fields in table like properties of an object 
  - all records in database have to conform with this schema
  - schema is like a unified way to organize data
  - a set of rules data must conform to 

5. What is a NoSQL database?
  - MongoDB 
  - in the database there are 
    1. collections
    2. documents: can have different structure/schema

6. How does it work?
  - stores data in structure that doesn't conform to one practice but a dynamic storage of data to allow more flexibility and do not have relations between documents/collections

7. What is inside of a Mongo database?
  - collections and documents

8. Which is more flexible - SQL or MongoDB? and why.
  - MongoDB: allows storage of data without requiring specific properties/documents to 
9. What is the disadvantage of a NoSQL database?
  - Schema-less, can't rely on record of a certain schema feild
  - no relations - must duplicate data
  - data is merged/nested in a few collections (this goal is to have all the data in one collection)
  - scales vertically and horizontally 