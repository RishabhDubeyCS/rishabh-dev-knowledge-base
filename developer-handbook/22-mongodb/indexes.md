# indexes

## Purpose

Improve query performance.

---

## Create Index

```javascript
db.users.createIndex({
  email: 1
})
```

---

## View Indexes

```javascript
db.users.getIndexes()
```

---

## Remove Index

```javascript
db.users.dropIndex("email_1")
```

---

## Why Use Indexes?

Without index:

```javascript
db.users.find({
  email: "user@example.com"
})
```

MongoDB scans every document.

With index:

MongoDB directly finds matching records.

---

## Cheat Sheet

```javascript
createIndex()
getIndexes()
dropIndex()
```
 