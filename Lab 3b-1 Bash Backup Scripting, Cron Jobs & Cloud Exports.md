# 3b-1 Bash Backup Scripting, Cron Jobs & Cloud Exports

## Practice some bash commands
I practiced some basic Bash commands like echo, variables, arithmetic using (( )), and a for loop to calculate a sum.
<img width="600" alt="image" src="https://github.com/user-attachments/assets/c5e6fae8-dc04-4269-a357-ba77c7a4d296" />

## Test Files & Directories
Next is I created some folders and test files inside the Documents directory to use in the automated backup script.
<img width="600" alt="image" src="https://github.com/user-attachments/assets/e128f614-25ba-4d1b-a890-d2dbe120ce05" />

## Basic Bash Script
I created and also tested a bash script that copies the contents of the documents directory into the backup directory.
<img width="600" alt="image" src="https://github.com/user-attachments/assets/d71e4bbf-650f-446c-a207-e48ccde8a5c1" />

## Move script to /usr/bin
I moved the testscript to /usr/bin and changed the ownership to root. I successfully executed the script from another directory, which shows a system-wide availability.
<p><img width="600" alt="image" src="https://github.com/user-attachments/assets/fe58a5a1-a07d-489e-bb79-8b5920123e65" /></p>

## Zip Archive with date filename
Next, I updated the bash script to create a compressed zip archive of the backup directory. The filename now uses a current date generated with the date command.
<p><img width="600" alt="image" src="https://github.com/user-attachments/assets/89dff4fd-63fd-481d-8b3d-3405bfc13dc0" /></p>

## Cron job setup
I added an hourly cron job which automatically executes /usr/bin/testscript at 9 minutes past every hour.
<img width="600" alt="image" src="https://github.com/user-attachments/assets/5c3527d8-06b8-4ae2-bf38-06b471d38ea2" />

## Verify Cron Execution
So here I verified the backup script successfully created a timestamp zip archives. The file name all include time and date.
<p><img width="600" alt="image" src="https://github.com/user-attachments/assets/0e7726b0-7117-49ac-b4b3-9e7ac374f25f" /></p>

## SCP to Cloud
