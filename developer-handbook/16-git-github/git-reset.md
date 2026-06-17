# git reset

## Purpose

Undo changes or commits.

---

## Unstage Files

```bash
git reset file.txt
```

---

## Undo Last Commit

Keep changes:

```bash
git reset --soft HEAD~1
```

---

## Remove Commit & Changes

```bash
git reset --hard HEAD~1
```

⚠️ Deletes changes permanently.

---

## Cheat Sheet

```bash
git reset file.txt
git reset --soft HEAD~1
git reset --hard HEAD~1
```
 