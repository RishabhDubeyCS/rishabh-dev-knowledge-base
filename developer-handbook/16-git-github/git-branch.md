# git branch

## Purpose

Create and manage branches.

---

## Why Branches?

```text
main
 ├── feature-auth
 ├── feature-payment
 └── feature-dashboard
```

Each feature gets its own branch.

---

## View Branches

```bash
git branch
```

---

## Create Branch

```bash
git branch feature-auth
```

---

## Switch Branch

```bash
git checkout feature-auth
```

---

## Create & Switch

```bash
git checkout -b feature-auth
```

---

## Delete Branch

```bash
git branch -d feature-auth
```

---

## Cheat Sheet

```bash
git branch
git checkout -b feature-auth
git branch -d feature-auth
```
 