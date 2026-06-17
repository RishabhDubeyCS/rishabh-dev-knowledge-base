# restore

## Purpose

Restore MongoDB databases from backups.

---

## Restore Database

```bash
mongorestore backup/mydb
```

---

## Restore All Databases

```bash
mongorestore backup/
```

---

## Drop Existing Data Before Restore

```bash
mongorestore --drop backup/mydb
```

---

## Cheat Sheet

```bash
mongorestore backup/mydb
mongorestore backup/
mongorestore --drop backup/mydb
```
 