# Laboratory Activity 9 

## Mission Overview

Congratulations! Your ability to secure cloud environments has proven you are ready for the highest
level of operations. You have been promoted to the Cloud Automation and DevOps Team at CloudNova
Technologies.
Up until now, you have been acting as a traditional systems administrator—typing commands manually
one by one. In large enterprise environments scaling to thousands of servers, manual administration is too slow
and highly prone to human error. To survive at scale, you must learn to automate.
Using the KillerCoda Playground, you will step into the role of a Cloud Automation Engineer. You will
learn the basics of Bash shell scripting, create an automated backup routine, assign executable permissions, and
configure the Linux Cron scheduler to run your code autonomously.
Remember: If you have to do a task more than twice in the cloud, you should automate it.
## Mission Objectives

At the end of this laboratory activity, you should be able to:
- Understand the fundamental syntax of a Bash shell script, including variables and basic commands.
- Use a command-line text editor (nano) to write and save executable scripts.
- Modify Linux file permissions using the chmod command.
- Understand task scheduling and the syntax of a Linux crontab.
- Document automation code and Cron job configurations using Markdown.
- Complete the final chapter of your GitHub Cloud Computing Portfolio. 

## Commands Executed

**Create a dummy folder with a test file inside it to represent the client's data.**
```
mkdir app-data
echo "This is critical client data." > app-data/data.txt 
```
**Open the Linux terminal text editor (nano) to create your automation script.**
```
nano backup.sh
```
**Copy the following Bash code and paste it into the nano editor.**
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
**Attempt to run the script normally. You will see a "Permission denied" error**
```
./backup.sh
```
**Change the file permissions to make the script executable using chmod**
```
chmod +x backup.sh
```

**Run the script again. It will now execute successfully**
```
./backup.sh 
```
**Verify that the script actually created the backup folder and the compressed file**
```
ls -l backups/ 
```
**Check your current active cron jobs by typing**
```
crontab -l
```
**Open the cron table editor by typing**
```
env EDITOR=nano crontab -e
```

**Scroll to the very bottom of the file (past all the # comments) and add the following line. This tells the
system to run your script every single night at exactly 2:00 AM**
```
0 2 * * * /root/backup.sh
```

## Skills Learned

- **Bash Shell Scripting:** Mastered the fundamental syntax of Bash scripts, including utilizing variables (\$BACKUP_DIR), dynamic timestamps (\$(date)), and condition checking to streamline routine administrative tasks.
- **Command-Line Text Editing:** Gained proficiency in using terminal-based text editors (nano) to create, edit, save, and manage configuration and script files directly within an Ubuntu cloud environment.
- **Linux File Permission Management:** Learned how to modify file execution rights using the chmod +x command to safely transition text files into executable programs.
- **Task Automation and Cron Scheduling:** Understood the architecture of time-based job scheduling in Linux, mastering crontab syntax (0 2 * * *) to automate critical operations like nightly server backups without manual intervention.
- **Cloud Infrastructure Documentation:** Developed comprehensive Markdown documentation and technical guides detailing script functions, permission controls, and cron expressions for client IT teams.
