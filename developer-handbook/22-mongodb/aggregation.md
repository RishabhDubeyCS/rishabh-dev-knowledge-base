# aggregation

## Purpose

Analyze and transform data using pipelines.

---

## Syntax

```javascript
db.collection.aggregate([
  { stage }
])
```

---

## Example

Group users by department:

```javascript
db.users.aggregate([
  {
    $group: {
      _id: "$department",
      total: { $sum: 1 }
    }
  }
])
```

---

## Common Stages

### Match

```javascript
{
  $match: {
    age: { $gte: 18 }
  }
}
```

### Group

```javascript
{
  $group: {
    _id: "$role",
    count: { $sum: 1 }
  }
}
```

### Sort

```javascript
{
  $sort: {
    age: -1
  }
}
```

### Project

```javascript
{
  $project: {
    name: 1,
    age: 1
  }
}
```

---

## Cheat Sheet

```javascript
$match
$group
$sort
$project
$lookup
```
 