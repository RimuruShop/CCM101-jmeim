# Automation Research

## Bash Script

A Bash script is a text file that contains multiple Linux commands arranged in a specific order. When executed, the shell runs each command one after another, just like a user entering them manually in the terminal. The `#!/bin/bash` line at the beginning is known as the shebang. It tells the operating system to use Bash as the interpreter for executing the commands inside the script.

## Variables

Variables such as `$BACKUP_DIR` are used to store values like folder paths so programmers do not have to write the same information repeatedly. This makes scripts easier to manage and reduces mistakes. If the backup folder needs to be changed, the programmer only has to modify the variable's value instead of updating every command that uses it.

## Cron Job

A cron job is an automated task managed by Linux's cron service that runs a command or script according to a specific schedule. It can execute tasks at certain times, dates, or repeated intervals without requiring manual input. This is useful in cloud operations because regular activities, such as creating backups, can run automatically without someone needing to remember to perform them every day.
