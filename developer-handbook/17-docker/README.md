real developer workflow:

Build → Run → Logs → Exec → Volumes → Networks → Compose → Troubleshooting 

# README

## Purpose

Learn Docker from beginner to developer level by understanding how containers are built, run, debugged, connected, and deployed.

---

# What is Docker?

Docker is a platform that allows you to package your application and all its dependencies into a container.

Think of Docker as:

```text
Code + Dependencies + Runtime
            ↓
        Docker Image
            ↓
      Docker Container
```

Without Docker:

```text
Works on my machine not 
Fails on production  not 
```

With Docker:

```text
Works everywhere ✅
```

---

# Real-World Analogy

Imagine:

```text
Image = Cake Recipe
Container = Actual Cake
```

You can create many cakes (containers) from one recipe (image).

---

# Learning Path

## Step 1: Run Existing Containers

* docker-run.md

Learn how to start containers.

---

## Step 2: View Container Logs

* docker-logs.md

Learn how to debug running containers.

---

## Step 3: Enter Running Containers

* docker-exec.md

Learn how to inspect and troubleshoot containers.

---

## Step 4: Build Your Own Images

* docker-build.md

Learn how to package applications.

---

## Step 5: Persist Data

* docker-volume.md

Learn how to save database data.

---

## Step 6: Connect Containers

* docker-network.md

Learn how applications communicate.

---

## Step 7: Run Multi-Container Apps

* docker-compose.md

Run Node.js + MongoDB + Redis together.

---

## Step 8: Troubleshooting

* troubleshooting.md

Fix common Docker problems.

---

# Recommended Order

1. docker-run
2. docker-logs
3. docker-exec
4. docker-build
5. docker-volume
6. docker-network
7. docker-compose
8. troubleshooting

---

# Summary (Hinglish)

Docker ek technology hai jo application ko container ke andar run karti hai.

Image = Blueprint

Container = Running Application

Real-world workflow:

Build → Run → Logs → Exec → Volume → Network → Compose

Agar Docker samajh gaya to deployment aur production kaafi easy ho jaata hai.
 