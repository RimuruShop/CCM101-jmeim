# Laboratory Activity 9: Mission 9 – The Cloud Automation Engineer

## Mission Overview

This laboratory activity focuses on automating regular server tasks to reduce manual work and avoid human errors. It involves creating a Bash script that compresses and saves a backup of application data, then using Linux cron to schedule the script to run automatically every day at 2:00 AM without requiring manual execution.

## Objectives

- Learn the basic structure and syntax of Bash scripts, including variables and commands.
- Use the nano editor to create, edit, and save an executable script.
- Apply the correct file permissions using the chmod command.
- Understand how to schedule automated tasks using Linux crontab.
- Record automation scripts and scheduling configurations using Markdown.

## Commands Executed

- `mkdir app-data` / `echo "..." > app-data/data.txt` — created a sample folder and file containing test data.
- `nano backup.sh` — opened the nano editor to create the backup script.
- `chmod +x backup.sh` — gave the script permission to execute.
- `./backup.sh` — executed the script to generate a compressed backup file in `.tar.gz` format.
- `crontab -e` — edited the cron schedule and added an entry to run the backup script every day at 2:00 AM.
- `crontab -l` — displayed the current cron configuration to confirm that the scheduled task was saved.

## Skills Learned

- Creating and running Bash scripts using the Linux terminal.
- Setting and modifying file permissions through the chmod command.
- Automating repeated tasks using the Linux cron scheduler.
- Understanding how scheduled scripts help reduce manual work and human errors.
- Documenting automation procedures and cron configurations for future reference.
