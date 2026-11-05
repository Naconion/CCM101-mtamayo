# Technical Documentation

## Full Code of my backup.sh script
```
#!/bin/bash
# Automated Backup Script for CloudNova Technologies
SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")
echo "Initiating automated backup..."
# Create the backup directory if it does not exist
mkdir -p $BACKUP_DIR
# Compress the source directory into a tarball (.tar.gz)
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR
echo "Backup completed successfully at $TIMESTAMP!"
```

## Explaination on what the chmod +x command did to the file.
It changes file permissions to make the text file executable as a program.

## What each of the five time-fields means (Minute, Hour, Day of Month, Month, Day of Week). 

- Minute (0): Minute of the hour (0–59) -> 0th minute.

- Hour (2): Hour of the day in 24-hour format (0–23) -> 2:00 AM.

- Day of Month (*): Day of the month (1–31) -> Every day.

- Month (*): Month of the year (1–12) -> Every month.

- Day of Week (*): Day of the week (0–7, where 0 and 7 are Sunday) -> Every day of the week.
