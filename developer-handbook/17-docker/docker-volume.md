# docker volume

## Purpose

Store data permanently.

---

## Problem

Container delete:

```bash
docker rm container
```

Data bhi delete ❌

---

## Solution

Create volume:

```bash
docker volume create mongodb-data
```

---

## Attach Volume

```bash
docker run -v mongodb-data:/data/db mongo
```

---

## View Volumes

```bash
docker volume ls
```

---

## Summary (Hinglish)

Volume data ko container ke bahar store karta hai.

Container delete ho sakta hai.

Data safe rehta hai.
