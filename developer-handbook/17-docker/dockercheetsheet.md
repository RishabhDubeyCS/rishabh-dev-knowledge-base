# Docker Cheat Sheet

> Quick reference for daily Docker development, debugging, deployment, and production operations.

---

# Docker Information

```bash
docker --version
docker version
docker info
docker help
docker system df
docker system events
```

---

# Images

## Pull Image

```bash
docker pull nginx
docker pull node:22
docker pull mongo:8
```

## List Images

```bash
docker images
docker image ls
```

## Inspect Image

```bash
docker inspect nginx
```

## Tag Image

```bash
docker tag my-app:latest username/my-app:v1
```

## Remove Image

```bash
docker rmi image-id
```

## Save Image

```bash
docker save -o app.tar my-app
```

## Load Image

```bash
docker load -i app.tar
```

---

# Containers

## Run Container

```bash
docker run nginx
docker run -d nginx
docker run -p 8080:80 nginx
docker run --name my-nginx nginx
```

## List Containers

```bash
docker ps
docker ps -a
```

## Start Container

```bash
docker start container-id
```

## Stop Container

```bash
docker stop container-id
```

## Restart Container

```bash
docker restart container-id
```

## Kill Container

```bash
docker kill container-id
```

## Pause Container

```bash
docker pause container-id
```

## Resume Container

```bash
docker unpause container-id
```

## Rename Container

```bash
docker rename old-name new-name
```

## Remove Container

```bash
docker rm container-id
docker rm -f container-id
```

---

# Logs & Debugging

## View Logs

```bash
docker logs container-name
```

## Live Logs

```bash
docker logs -f container-name
```

## Last 100 Lines

```bash
docker logs --tail 100 container-name
```

## Open Shell

```bash
docker exec -it container-name bash
docker exec -it container-name sh
```

## View Running Processes

```bash
docker top container-name
```

## Resource Usage

```bash
docker stats
```

## Inspect Container

```bash
docker inspect container-name
```

---

# Docker Build

## Build Image

```bash
docker build -t my-app .
```

## Build Specific Dockerfile

```bash
docker build -f Dockerfile.prod -t my-app .
```

## Build Without Cache

```bash
docker build --no-cache -t my-app .
```

## Build Multi Platform

```bash
docker buildx build --platform linux/amd64,linux/arm64 .
```

---

# Dockerfile Essentials

```dockerfile
FROM node:22

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD ["npm","start"]
```

---

# Volumes

## Create Volume

```bash
docker volume create mongodb-data
```

## List Volumes

```bash
docker volume ls
```

## Inspect Volume

```bash
docker volume inspect mongodb-data
```

## Mount Volume

```bash
docker run -v mongodb-data:/data/db mongo
```

## Remove Volume

```bash
docker volume rm mongodb-data
```

---

# Bind Mounts

```bash
docker run \
-v $(pwd):/app \
node:22
```

Windows:

```bash
docker run -v ${PWD}:/app node:22
```

---

# Networks

## Create Network

```bash
docker network create app-network
```

## List Networks

```bash
docker network ls
```

## Inspect Network

```bash
docker network inspect app-network
```

## Connect Container

```bash
docker network connect app-network container-name
```

## Remove Network

```bash
docker network rm app-network
```

---

# Docker Compose

## Start Services

```bash
docker compose up
```

## Start In Background

```bash
docker compose up -d
```

## Stop Services

```bash
docker compose down
```

## View Logs

```bash
docker compose logs
docker compose logs -f
```

## Execute Command

```bash
docker compose exec app bash
```

## Rebuild

```bash
docker compose up --build
```

---

# Registry Operations

## Login

```bash
docker login
```

## Logout

```bash
docker logout
```

## Push Image

```bash
docker push username/app:v1
```

## Pull Image

```bash
docker pull username/app:v1
```

---

# Resource Management

## Limit Memory

```bash
docker run -m 512m nginx
```

## Limit CPU

```bash
docker run --cpus=1 nginx
```

## Restart Policy

```bash
docker run --restart always nginx
```

---

# Cleanup Commands

## Remove Stopped Containers

```bash
docker container prune
```

## Remove Unused Images

```bash
docker image prune
```

## Remove Unused Volumes

```bash
docker volume prune
```

## Remove Unused Networks

```bash
docker network prune
```

## Remove Everything Unused

```bash
docker system prune -a
```

---

# Troubleshooting

## Check Containers

```bash
docker ps -a
```

## Check Logs

```bash
docker logs container-name
```

## Check Resource Usage

```bash
docker stats
```

## Check Docker Disk Usage

```bash
docker system df
```

## Port Conflict

Linux:

```bash
lsof -i :3000
```

Windows:

```bash
netstat -ano | findstr :3000
```

---

# Production Commands

## Backup MongoDB

```bash
docker exec mongodb mongodump --out /backup
```

## Copy Files From Container

```bash
docker cp container:/app/logs ./logs
```

## Copy Files To Container

```bash
docker cp config.json container:/app
```

## Export Container

```bash
docker export container-id > container.tar
```

## Import Container

```bash
docker import container.tar my-image
```

---

# Daily Developer Workflow

```bash
docker compose up -d

docker ps

docker logs -f app

docker exec -it app bash

docker compose down
```

---

# Most Important Commands

```bash
docker pull
docker build
docker run
docker ps
docker logs
docker exec
docker stop
docker rm

docker volume ls
docker network ls

docker compose up -d
docker compose down

docker image prune
docker system prune -a
```

---

# Summary (Hinglish)

```text
Docker ka basic flow:

Image Pull Karo
↓
Container Run Karo
↓
Logs Check Karo
↓
Container Ke Andar Jao (exec)
↓
Volume Se Data Save Rakho
↓
Network Se Containers Connect Karo
↓
Compose Se Multiple Services Chalao

Daily Commands:

docker build
docker run
docker ps
docker logs
docker exec
docker compose up -d

Agar koi issue aaye:

docker ps -a
docker logs
docker inspect
docker stats

Ye 90% Docker problems solve kar dete hain.
```
 