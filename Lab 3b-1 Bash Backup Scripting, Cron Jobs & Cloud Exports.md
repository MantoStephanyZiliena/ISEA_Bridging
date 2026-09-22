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
<img width="600" alt="image" src="https://github.com/user-attachments/assets/e4912d6c-e0d9-4c24-80c7-ba3e2a5e9636" />
<img width="600" alt="image" src="https://github.com/user-attachments/assets/e3c9abec-3951-467e-b7a8-d58542f18748" />

## SSH Certificate Accepted by Root
I used SSH with the AWS private key to securely connect to the cloud server. The SSH host fingerprint was accepted and the connection was successfully established.
<p><img width="600" alt="Screenshot 2026-09-22 101930" src="https://github.com/user-attachments/assets/c0b5eb55-3323-415e-8c30-9f9dbcedd25d" /></p>

## Final Script
<img width="600" alt="Screenshot 2026-09-22 102744" src="https://github.com/user-attachments/assets/9c0cf389-3a7f-43b7-bbe0-55efe53f11ed" />


