
### xargs.md

```md
# xargs

## Purpose

Build and execute commands from input.

---

## Syntax

```bash
command | xargs [command] 

Examples
cat files.txt | xargs rm
Cheat Sheet
find . -name "*.log" | xargs rm
cat list.txt | xargs echo