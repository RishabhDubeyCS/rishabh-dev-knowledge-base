# docker logs

## Purpose

See what is happening inside a container.

---

## View Logs

```bash
docker logs my-container
```

---

## Live Logs

```bash
docker logs -f my-container
```

---

## Last 50 Lines

```bash
docker logs --tail 50 my-container
```

---

## Summary (Hinglish)

Application crash ho rahi hai?

docker logs sabse pehle check karo.

Ye container ka console output dikhata hai.
