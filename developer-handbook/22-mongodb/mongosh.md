# mongosh

## Purpose

`mongosh` (MongoDB Shell) is the command-line tool used to connect to MongoDB and execute database commands.

Think of it as:

```text
MySQL    → mysql
PostgreSQL → psql
MongoDB  → mongosh
```

---

## Prerequisites

Make sure MongoDB is installed.

Check if `mongosh` is available:

```bash
mongosh --version
```

Example Output:

```bash
2.5.8
```

---

## Step 1: Start MongoDB

If MongoDB is running locally:

```bash
mongosh
```

Expected Output:

```bash
Current Mongosh Log ID: ...
Connecting to: mongodb://127.0.0.1:27017/
```

You are now connected to MongoDB.

---

## Step 2: View Existing Databases

```javascript
show dbs
```

Example Output:

```text
admin     40 KB
config   108 KB
local     72 KB
```

---

## Step 3: Create or Switch Database

```javascript
use company
```

Output:

```text
switched to db company
```

If the database doesn't exist, MongoDB creates it when you insert data.

---

## Step 4: Check Current Database

```javascript
db
```

Output:

```text
company
```

---

## Step 5: Create Your First Collection

Insert a document:

```javascript
db.users.insertOne({
  name: "Rishabh",
  age: 22,
  role: "Developer"
})
```

Output:

```javascript
{
  acknowledged: true,
  insertedId: ObjectId("...")
}
```

MongoDB automatically creates:

```text
Database: company
Collection: users
```

---

## Step 6: View Collections

```javascript
show collections
```

Output:

```text
users
```

---

## Step 7: Read Data

Show all documents:

```javascript
db.users.find()
```

Pretty format:

```javascript
db.users.find().pretty()
```

Output:

```javascript
{
  _id: ObjectId("..."),
  name: "Rishabh",
  age: 22,
  role: "Developer"
}
```

---

## Step 8: Find One Document

```javascript
db.users.findOne({
  name: "Rishabh"
})
```

---

## Step 9: Update Data

```javascript
db.users.updateOne(
  { name: "Rishabh" },
  {
    $set: {
      age: 23
    }
  }
)
```

Verify:

```javascript
db.users.find().pretty()
```

---

## Step 10: Delete Data

Delete one document:

```javascript
db.users.deleteOne({
  name: "Rishabh"
})
```

Verify:

```javascript
db.users.find()
```

---

## Step 11: Count Documents

```javascript
db.users.countDocuments()
```

Output:

```text
5
```

---

## Step 12: Database Statistics

```javascript
db.stats()
```

Shows:

* Collection count
* Storage size
* Index size
* Document count

---

## Step 13: Exit mongosh

```javascript
exit
```

or

```javascript
.quit
```

---

## Real-World Developer Workflow

```bash
mongosh
```

```javascript
show dbs
use company
show collections

db.users.find().pretty()

db.users.insertOne({
  name: "John",
  email: "john@example.com"
})

db.users.find()

db.stats()

exit
```

---

## Most Important Commands

```javascript
show dbs
use mydb
db

show collections

db.users.find()
db.users.findOne()

db.users.insertOne()

db.users.updateOne()

db.users.deleteOne()

db.stats()

exit
```

---

## Beginner Roadmap

```text
1. mongosh
2. show dbs
3. use mydb
4. insertOne()
5. find()
6. findOne()
7. updateOne()
8. deleteOne()
9. createIndex()
10. aggregate()
```

Master these first before moving to CRUD, Indexes, and Aggregation.
