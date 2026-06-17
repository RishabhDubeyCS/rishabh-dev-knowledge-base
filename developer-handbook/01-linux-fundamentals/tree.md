# tree

## Purpose

Display files and directories in a tree-like structure.

---

## Syntax

```bash
tree [options] [directory]
```

---

## Examples

```bash
tree
```

Show the current directory structure.

```bash
tree src
```

Show the structure of the `src` directory.

---

## Common Usage

```bash
tree          # Current directory
tree src      # Specific directory
tree -L 2     # Show 2 levels deep
tree -a       # Include hidden files
```

---

## Tips

* Great for visualizing project structure.
* Use `tree -L 2` to avoid very long output.
* Install if missing:

```bash
sudo apt install tree
```

---

## Related Commands

* `pwd` → Show current directory
* `cd` → Change directory
* `ls` → List files and folders

---

## Cheat Sheet

```bash
tree       # Show directory tree
tree src   # Show src folder tree
tree -L 2  # Limit depth to 2 levels
tree -a    # Include hidden files
```
