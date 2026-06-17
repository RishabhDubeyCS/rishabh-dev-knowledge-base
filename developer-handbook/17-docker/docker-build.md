# docker build

## Purpose

Create a Docker Image from your application.

---

## Real-World Analogy

```text
Source Code → Dockerfile → Docker Image
```

Image ek packaged version hota hai jo kisi bhi machine par run ho sakta hai.

---

## Step 1: Create Dockerfile

```dockerfile
FROM node:22

WORKDIR /app

COPY . .

RUN npm install

CMD ["npm", "start"]
```

---

## Step 2: Build Image

```bash
docker build -t my-app .
```

---

## Step 3: Verify

```bash
docker images
```

---

## Step 4: Run

```bash
docker run my-app
```

---

## Summary (Hinglish)

docker build application ka package banata hai.

Dockerfile recipe hoti hai.

docker build image create karta hai.

docker run image ko container me convert karta hai.
 