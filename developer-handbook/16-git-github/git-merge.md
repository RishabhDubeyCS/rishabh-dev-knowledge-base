# git merge

## Purpose

Combine changes from one branch into another.

---

## Scenario

```text
main
 └── feature-auth
```

Feature is completed.

---

## Step 1

Switch to main:

```bash
git checkout main
```

---

## Step 2

Merge feature branch:

```bash
git merge feature-auth
```

---

## Result

```text
main now contains feature-auth changes
```

---

## Cheat Sheet

```bash
git checkout main
git merge feature-auth
```
 