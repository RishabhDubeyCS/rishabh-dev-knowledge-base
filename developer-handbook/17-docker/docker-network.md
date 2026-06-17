# docker network

## Purpose

Allow containers to communicate.

---

## Create Network

```bash
docker network create app-network
```

---

## Connect MongoDB

```bash
docker run -d \
--network app-network \
mongo
```

---

## Connect Backend

```bash
docker run -d \
--network app-network \
backend
```

---

## Verify

```bash
docker network ls
```

---

## Summary (Hinglish)

Network containers ko connect karta hai.

Backend MongoDB se baat kar sakta hai.

Frontend Backend se connect ho sakta hai.
 