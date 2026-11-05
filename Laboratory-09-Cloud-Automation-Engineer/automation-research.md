# Checkpoint 2: Research - The Language of Automation

### 1. Bash Script
A Bash script is a plain-text file containing a sequence of commands executed line-by-line by the Bash shell interpreter to automate command-line workflows. The `#!/bin/bash` line at the very beginning is known as the shebang. It tells the operating system kernel which program interpreter (`/bin/bash`) must be used to parse and run the script[cite: 2].

### 2. Variables
Variables (such as `$BACKUP_DIR` and `$SOURCE_DIR`) are named pointers used to store values, paths, or command outputs dynamically[cite: 2, 3]. Cloud engineers use them instead of typing out repetitive static paths to prevent syntax errors, improve readability, and allow system paths to be changed across an entire script from a single variable definition[cite: 2].

### 3. Cron Job
A cron job is an automated background task managed by the Linux Cron daemon (`crond`) that runs commands or scripts at scheduled dates, times, or intervals. It is essential for cloud operations because it ensures critical routines—such as data backups, log maintenance, and patching—execute consistently without requiring manual human effort[cite: 1, 2].
