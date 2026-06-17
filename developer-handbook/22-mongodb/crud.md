# CRUD

## Purpose

Perform Create, Read, Update, and Delete operations.

---

## Create

Insert one document:

```javascript
db.users.insertOne({
  name: "Rishabh",
  age: 22
})
```

---

## Read

Find all documents:

```javascript
db.users.find()
```

Find one:

```javascript
db.users.findOne({ name: "Rishabh" })
```

---

## Update

```javascript
db.users.updateOne(
  { name: "Rishabh" },
  { $set: { age: 23 } }
)
```

---

## Delete

```javascript
db.users.deleteOne({
  name: "Rishabh"
})
```

---

## Cheat Sheet

```javascript
insertOne()
find()
findOne()
updateOne()
deleteOne()
```
 