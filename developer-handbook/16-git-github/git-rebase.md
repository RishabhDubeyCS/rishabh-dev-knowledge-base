# git rebase

## Purpose

Move commits onto another branch.

---

## Why Rebase?

Keeps history clean.

---

## Example

```bash
git checkout feature-auth
git rebase main
```

---

## Before

```text
main
 \
  feature-auth
```

---

## After

```text
main
  \
   feature-auth (updated)
```

---

## Continue After Conflict

```bash
git rebase --continue
```

---

## Abort

```bash
git rebase --abort
```

---

## Cheat Sheet

```bash
git rebase main
git rebase --continue
git rebase --abort
```
 