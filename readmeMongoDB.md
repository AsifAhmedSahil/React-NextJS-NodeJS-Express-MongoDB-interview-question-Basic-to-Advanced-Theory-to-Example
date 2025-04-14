# MongoDB
## What is MongoDB?

MongoDB is a NoSQL database that stores data in flexible, JSON-like documents, making it easy to scale and store unstructured data.

## What is the difference between MongoDB and a relational database?

MongoDB: Uses collections and documents instead of tables and rows. It is schema-less and stores data in a more flexible format.
Relational databases: Use tables, rows, and columns to store structured data with predefined schemas.
## What is a collection in MongoDB?

A collection is a grouping of MongoDB documents. It is similar to a table in a relational database.

## What is a document in MongoDB?

A document is a record in MongoDB, represented as a JSON-like object with key-value pairs. It’s similar to a row in a relational database.





## How do you connect to a MongoDB database?

You can connect to MongoDB using the MongoDB Node.js driver or Mongoose. Here's an example with Mongoose:

```js
Copy
const mongoose = require('mongoose');
mongoose.connect('mongodb://localhost/mydb', { useNewUrlParser: true, useUnifiedTopology: true });
```
## What is Mongoose?

Mongoose is an Object Data Modeling (ODM) library for MongoDB and Node.js. It provides a higher-level abstraction for working with MongoDB.

## What are MongoDB CRUD operations?

CRUD stands for Create, Read, Update, and Delete operations:

Create: Insert data into a collection (e.g., insertOne(), insertMany()).
Read: Retrieve data from a collection (e.g., find(), findOne()).
Update: Modify existing data (e.g., updateOne(), updateMany()).
Delete: Remove data from a collection (e.g., deleteOne(), deleteMany()).
## What is an index in MongoDB?

An index in MongoDB is a special data structure that improves the speed of query operations.

## What are the data types supported in MongoDB?

MongoDB supports various data types including String, Number, Boolean, Date, Array, Object, Null, and more.

## What is the _id field in MongoDB?

The _id field is a unique identifier automatically added to each document. It’s typically an ObjectId, but you can specify your own.

## What is the aggregation framework in MongoDB?

The aggregation framework is a powerful tool in MongoDB for processing and transforming data, allowing you to perform complex queries and operations like grouping, filtering, and sorting.

## What is a replica set in MongoDB?

A replica set is a group of MongoDB servers that maintain the same data set. One member is the primary, while the others are secondaries that replicate data from the primary.

## What is sharding in MongoDB?

Sharding is the process of distributing data across multiple servers to handle large-scale data sets and high throughput operations.

## What is the difference between find() and findOne() in MongoDB?

find(): Returns an array of documents that match the query.
findOne(): Returns a single document that matches the query.
## What is the insert() method in MongoDB?

The insert() method is used to add new documents to a collection.

## How do you update documents in MongoDB?

You can update documents using methods like updateOne(), updateMany(), or findOneAndUpdate().

## What is a MongoDB ObjectId?

ObjectId is a 12-byte identifier that is used to uniquely identify documents in a collection. It is the default value for the _id field.

## How do you delete documents in MongoDB?

You can delete documents using methods like deleteOne() and deleteMany().

## What is MongoDB’s MapReduce?

MapReduce is a data processing paradigm in MongoDB that allows you to process large data sets in parallel, using a map function and a reduce function.

## What is db.collection.createIndex() in MongoDB?

This method is used to create indexes on collections to optimize query performance.

