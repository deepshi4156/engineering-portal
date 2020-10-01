Indexes in any database are essential in improving the performance of their data retrieval speed, and the same is true for MongoDB. By using indexes, performance in MongoDB queries becomes more efficient. In this chapter, you will learn about the different indexing techniques and their limitations.

----> Indexing Array Fields

Let us consider a situation where you wish to look for user documents depending on the user's tags. For this, you have to create an index on your tag array within your collection. For building an index based array, you have to create separate index entries for each of its fields. Let us see how it can be implemented.

If you consider the below-mentioned document of users collection:

{
  "location": {
    "city": "Calgary, Alberta",
    "country": " Canada"
  },
  "tags": [
    "techwriter",
    "developer",
    "programmer"
  ],
  "name": "James Gosling"
}

For creating the index on tag array, you have to implement, i.e. execute the following code:

db.users.ensureIndex ( {"tags": 1} )

----> Indexing fields for Sub-Documents

Let us consider a situation where you wish to look for documents depending on the city and country fields (from the above example). As all the fields are part of the location sub-document field, you will have to generate an index on every field of sub-document. 
To create an index on each of the two fields of your sub-document, you have to make use of the below-mentioned code:

db.users.ensureIndex( {"location.city":1,"location.country":1} )

After creating an index, the search operation in any sub-document field can be performed using the index:

db.users.find({"location.city":"Los Angeles"})

----> Limitations and Threshold of Indexing in MongoDB

There are various limitations associated with indexing in MongoDB. These are:

- Extra Overhead: All of the indexes occupy certain space as well as bring a cost on every insertion, updating and deleting operations. Hence, if you hardly ever make use of your collection for reading operations, it does not make any sense of using indexes.
- RAM Usage: Because all of MongoDB indexes get stored in RAM, you must make sure that the entire size of your index doesn't go beyond the RAM limit. And, if such a scenario occurs, it will begin deleting some indexes, degrading the performance of indexing.
- Query Limitations: Indexing cannot be implemented in queries that make use of:
1. Regular expressions and or negation operators such as $nin, $not, etc.
2. The $where clause
3. Any arithmetic operators such as $mod, etc.
- Index Key Limits: In the earlier version, i.e. 2.6, MongoDB does not produce an index when the value of the obtainable index field goes beyond the limit of the index key.
- Indexes of a particular collection cannot exceed more than 64.
- Name Length of the index: The fully qualified name of the index that comprises of the namespace followed by the dot separators (which looks something like: <database name>.<collection name>.$<index name>), cannot go beyond the length of 128 characters.
- Quantity of Indexed Fields within a compound index cannot exceed more than 32 fields.
