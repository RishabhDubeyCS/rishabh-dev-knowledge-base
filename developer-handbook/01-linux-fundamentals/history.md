# history

## Purpose

Display previously executed commands.

---

## Syntax

```bash
history
```

---

## Examples

```bash
history
```

Output:

```bash
1  pwd
2  ls
3  cd project
4  git status
5  npm install
```

```bash
history 10
```

Show the last 10 commands.

---

## Common Usage

```bash
history      # Show command history
history 20   # Last 20 commands
```

---

## Tips

* Use the Up Arrow (↑) to quickly access previous commands.
* Search command history:

```bash
Ctrl + R
```

* Re-run a command by its number:

```bash
!25
```

Runs command number 25 from history.

---

## Related Commands

* `pwd` → Show current directory
* `ls` → List files and folders
* `clear` → Clear terminal screen

---

## Cheat Sheet

```bash
history      # Show all command history
history 10   # Show last 10 commands
Ctrl + R     # Search command history
!25          # Run command #25
```
