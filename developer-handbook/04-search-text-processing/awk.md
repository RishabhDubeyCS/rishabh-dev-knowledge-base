
### awk.md

```md
# awk

## Purpose

Process and analyze structured text.

---

## Syntax

```bash
awk 'pattern {action}' file 



Examples
awk '{print $1}' users.txt
Cheat Sheet
awk '{print $1}' file.txt
awk -F, '{print $2}' users.csv
awk '/error/' logs.txt 





### Test File

```bash
echo "apple" > demo.txt
echo "banana" >> demo.txt
echo "apple" >> demo.txt

Practice:

grep apple demo.txt
sort demo.txt
uniq demo.txt
cat demo.txt | tr a-z A-Z