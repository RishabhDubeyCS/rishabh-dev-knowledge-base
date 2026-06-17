ls         # List files
ls -l      # Detailed view
ls -a      # Show hidden files
ls -la     # Detailed + hidden files
ls -lh     # Human-readable sizes
ls -R      # Recursive listing
ls -ltr    # Sort by time
ls -lhS    # Sort by size

------------------------------------------------------------------

cd folder     # Enter folder
cd ..         # One level up
cd ~          # Home directory
cd -          # Previous directory
cd /          # Root directory

-----------------------------------------------
Cheat Sheet
tree       # Show directory tree
tree src   # Show src folder tree
tree -L 2  # Limit depth to 2 levels
tree -a    # Include hidden files 


-------------------------------------------

## Cheat Sheet

```bash
which python   # Find Python executable
which node     # Find Node.js executable
which npm      # Find NPM executable
which git      # Find Git executable
```

------------------------------------------------
## Cheat Sheet

```bash
history      # Show all command history
history 10   # Show last 10 commands
Ctrl + R     # Search command history
!25          # Run command #25 

-----------------------------------------
Cheat Sheet
alias ll='ls -lah'      # Detailed file listing
alias gs='git status'   # Git status
alias gp='git push'     # Git push
alias ..='cd ..'        # Go back one directory

alias                   # Show all aliases
alias ll                # Show specific alias
unalias ll              # Remove alias

nano ~/.bashrc          # Edit aliases
source ~/.bashrc        # Reload configuration