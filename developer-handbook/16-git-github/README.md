# README

## Purpose

Learn Git and GitHub from project initialization to branch management and collaboration.

---

## Learning Path

### Step 1: Initialize a Repository

* git-init.md

Learn how to start tracking a project with Git.

---

### Step 2: Clone Existing Repositories

* git-clone.md

Learn how to download repositories from GitHub.

---

### Step 3: Work with Branches

* git-branch.md

Create, switch, rename, and delete branches.

---

### Step 4: Merge Changes

* git-merge.md

Combine changes from one branch into another.

---

### Step 5: Save Work Temporarily

* git-stash.md

Store unfinished work without committing.

---

### Step 6: Rewrite History

* git-rebase.md

Keep commit history clean and linear.

---

### Step 7: Undo Changes

* git-reset.md

Remove commits or unstage files safely.

---

## Recommended Order

1. git-init
2. git-clone
3. git-branch
4. git-merge
5. git-stash
6. git-rebase
7. git-reset

---

## Real-World Workflow

```bash
git clone <repo>

git checkout -b feature/auth

# Make changes

git add .
git commit -m "feat: add auth"

git push origin feature/auth
```
 