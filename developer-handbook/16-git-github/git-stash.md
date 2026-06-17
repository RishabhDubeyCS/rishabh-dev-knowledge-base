# git stash

## Purpose

Temporarily save uncommitted work.

---

## Save Work

```bash
git stash
```

---

## View Stashes

```bash
git stash list
```

---

## Restore Latest

```bash
git stash pop
```

---

## Use Case

```text
Working on Feature A
Urgent Bug Fix Arrives
↓
git stash
Switch Branch
Fix Bug
Return
git stash pop
```

---

## Cheat Sheet

```bash
git stash
git stash list
git stash pop
```
 