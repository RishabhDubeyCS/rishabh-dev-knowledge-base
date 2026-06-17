# mongosh

## Purpose

Connect to and interact with MongoDB from the command line.

---

## Syntax

```bash
mongosh
```

---

## Examples

Connect to local MongoDB:

```bash
mongosh
```

Connect to MongoDB Atlas:

```bash
mongosh "mongodb+srv://cluster.mongodb.net/"
```

---

## Common Commands

Show databases:

```javascript
show dbs
```

Use a database:

```javascript
use company
```

Show collections:

```javascript
show collections
```

---

## Cheat Sheet

```javascript
show dbs
use mydb
show collections
db.stats()
```
 