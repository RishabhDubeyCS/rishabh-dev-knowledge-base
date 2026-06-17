# alias

## Purpose

Create custom shortcuts for long or frequently used commands.

---

## Syntax

```bash
alias name='command'
```

---

## Step 1: Create a Temporary Alias

Create a shortcut named `ll` for `ls -lah`:

```bash
alias ll='ls -lah'
```

Verify:

```bash
alias ll
```

Output:

```bash
alias ll='ls -lah'
```

---

## Step 2: Use the Alias

Run:

```bash
ll
```

Instead of:

```bash
ls -lah
```

---

## Step 3: Create More Useful Aliases

Git shortcuts:

```bash
alias gs='git status'
alias ga='git add .'
alias gc='git commit -m'
alias gp='git push'
```

Directory navigation:

```bash
alias ..='cd ..'
alias ...='cd ../..'
```

Node.js:

```bash
alias ni='npm install'
alias nr='npm run dev'
```

---

## Step 4: View All Aliases

Show every alias currently loaded:

```bash
alias
```

---

## Step 5: Remove an Alias

Remove a specific alias:

```bash
unalias ll
```

Verify:

```bash
alias ll
```

Output:

```bash
bash: alias: ll: not found
```

---

## Step 6: Make Aliases Permanent (Git Bash)

Open your Bash configuration file:

```bash
nano ~/.bashrc
```

Add:

```bash
alias ll='ls -lah'
alias gs='git status'
alias gp='git push'
alias ..='cd ..'
```

Save and exit:

```text
CTRL + O
ENTER
CTRL + X
```

Reload the configuration:

```bash
source ~/.bashrc
```

---

## Common Usage

```bash
alias ll='ls -lah'
alias gs='git status'
alias gp='git push'
alias ..='cd ..'
alias ni='npm install'
alias nr='npm run dev'
```

---

## Tips

* Aliases are available only in the current session unless saved in `.bashrc`.
* Use short, memorable names.
* Great for Git, Node.js, Docker, and Linux commands.
* Git Bash fully supports aliases.

---

## Related Commands

* `history` → Show command history
* `which` → Find command location
* `cd` → Change directory
* `source` → Reload shell configuration

---

## Cheat Sheet

```bash
alias ll='ls -lah'      # Detailed file listing
alias gs='git status'   # Git status
alias gp='git push'     # Git push
alias ..='cd ..'        # Go back one directory

alias                   # Show all aliases
alias ll                # Show specific alias
unalias ll              # Remove alias

nano ~/.bashrc          # Edit aliases
source ~/.bashrc        # Reload configuration
```
