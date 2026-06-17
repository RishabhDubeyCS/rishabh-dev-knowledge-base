# which

## Purpose

Show the location of an executable command.

---

## Syntax

```bash
which [command]
```

---

## Examples

```bash
which python
```

Output:

```bash
/c/Users/dubey/AppData/Local/Programs/Python/Python313/python
```

```bash
which node
```

Output:

```bash
/c/Program Files/nodejs/node
```

```bash
which git
```

Output:

```bash
/mingw64/bin/git
```

---

## Common Usage

```bash
which python
which node
which npm
which git
```

---

## Tips

* Useful for finding where a command is installed.
* Helps debug PATH-related issues.
* Available in Linux, macOS, and Git Bash.

---

## Related Commands

* `whereis` → Find binary, source, and manual files
* `where` → Windows equivalent
* `find` → Search files and directories

---

## Cheat Sheet

```bash
which python   # Find Python executable
which node     # Find Node.js executable
which npm      # Find NPM executable
which git      # Find Git executable
```
