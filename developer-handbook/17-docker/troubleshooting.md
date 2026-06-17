# Docker Troubleshooting

## Container Not Starting

Check:

```bash
docker ps -a
```

---

## View Error

```bash
docker logs container-name
```

---

## Port Already Used

Check:

```bash
netstat -ano | findstr :3000
```

---

## Clean Docker

```bash
docker system prune -a
```

---

## Summary (Hinglish)

Docker issue aaye to:

1. docker ps -a
2. docker logs
3. docker exec
4. docker system prune

Ye 90% Docker problems solve kar dete hain.
 