ls
Purpose

List files and directories in the current location.


 # Common Options 
| Option | Description                         |
| ------ | ----------------------------------- |
| `-l`   | Long listing format                 |
| `-a`   | Show hidden files                   |
| `-h`   | Human-readable file sizes           |
| `-R`   | Recursive listing                   |
| `-t`   | Sort by modification time           |
| `-S`   | Sort by file size                   |
| `-r`   | Reverse order                       |
| `-d`   | List directory itself, not contents |


Examples
List files and directories 

ls

Output:

Documents  Downloads  Pictures  file.txt
Long listing format
ls -l

Output:

-rw-r--r-- 1 user user 1200 Jun 17 file.txt
drwxr-xr-x 2 user user 4096 Jun 17 Documents
Show hidden files
ls -a

Output:

.  ..  .git  .env  file.txt
Human-readable file sizes
ls -lh

Output:

-rw-r--r-- 1 user user 1.2K Jun 17 file.txt
-rw-r--r-- 1 user user 2.5M Jun 17 video.mp4
List files recursively
ls -R

Output:

project/
├── src
├── public
└── package.json
Show only directories
ls -d */

Output:

Documents/
Downloads/
Pictures/
Useful Combinations
ls -lah     # Detailed view with hidden files
ls -ltr     # Sort by time (oldest first)
ls -lhS     # Sort by size (largest first)
ls -R       # Recursive listing
Real-World Usage

Check project files:

ls

Inspect a Next.js project:

ls -lah

View all files including hidden ones:

ls -a
Tips
Use ls -lah most often during development.
Hidden files start with a dot (.), such as .gitignore and .env.
Combine options together:
ls -lah

instead of:

ls -l -a -h


# Cheat Sheet

 ls         # List files
ls -l      # Detailed view
ls -a      # Show hidden files
ls -la     # Detailed + hidden files
ls -lh     # Human-readable sizes
ls -R      # Recursive listing
ls -ltr    # Sort by time
ls -lhS    # Sort by size 