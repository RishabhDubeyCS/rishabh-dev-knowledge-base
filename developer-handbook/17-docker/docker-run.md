# docker run

## Purpose

Create and start a container.

---

## Step 1

Run nginx:

```bash
docker run nginx
```

Docker automatically:

1. Downloads image
2. Creates container
3. Starts container

---

## Step 2

Run in background:

```bash
docker run -d nginx
```

---

## Step 3

Expose port:

```bash
docker run -d -p 8080:80 nginx
```

Open:

```text
http://localhost:8080
```

---

## Step 4

Check running containers:

```bash
docker ps
```

---

## Summary (Hinglish)

docker run image ko start karta hai.

-d = background me run

-p = port mapping

docker ps = running containers dekhne ke liye.
 