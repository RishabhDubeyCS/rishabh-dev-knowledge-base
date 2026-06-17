# Docker Compose

## Purpose

Run multiple containers together.

---

## Problem

Manually run:

```bash
docker run mongodb
docker run backend
docker run frontend
```

Difficult ❌

---

## Solution

docker-compose.yml

```yaml
services:
  mongo:
    image: mongo

  app:
    build: .
```

---

## Start Everything

```bash
docker compose up -d
```

---

## Stop Everything

```bash
docker compose down
```

---

## Summary (Hinglish)

Docker Compose multiple containers ko ek command se manage karta hai.

Production projects me almost har jagah use hota hai.
 