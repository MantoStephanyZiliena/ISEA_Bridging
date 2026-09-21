# 1b-2 Linux File Permissions and Group Access Control
## Created Users
I created the three users named Alice, Bob, and Mallory according to the lab activities instruction.
<img width="500" alt="Screenshot 2026-09-13 111157" src="https://github.com/user-attachments/assets/44b5865f-614c-4d00-b9dd-240ffb27b944" />

## Created a Group
Next I created a group where Alice and Bob are the members.
<p><img width="500" alt="Screenshot 2026-09-13 111446" src="https://github.com/user-attachments/assets/ad316b91-23f4-45ac-836a-b59f44cc7604" /></p>

## Created a Directory
Here I created the directory and using the command "sudo mkdir /home/shared? and verified it that the directory is successfully created.
<p><img width="500" alt="image" src="https://github.com/user-attachments/assets/84208e2c-0cbd-47b6-879a-319bb9b7b83c" /></p>


## Created Ten Files and Permissions Assigned
Here are the ten files are created inside "/home/shared". It also shows that Alice gets the Permission to be the group owner.
<p><img width="500" alt="Screenshot 2026-09-13 120333" src="https://github.com/user-attachments/assets/37493941-1ec9-4cc2-8e86-d33195670ca7" /></p>

## Access verified per User
For this part, Alice and Bob has gain access to the directory but Mallory is denied because she is not part of the group because I did not add her.

Alice:
<p><img width="500" alt="Screenshot 2026-09-13 120848" src="https://github.com/user-attachments/assets/8f04460e-fb3b-4687-8467-3f0a8e35875d" /></p>
Bob:
<p></p><img width="500" alt="Screenshot 2026-09-13 121113" src="https://github.com/user-attachments/assets/a6b7d5f8-0726-4a26-a98a-e3cec84ea6b4" /></p>
Mallory:
<p></p><img width="500" alt="Screenshot 2026-09-13 122147" src="https://github.com/user-attachments/assets/37c4fb46-b33d-4082-81fd-752410d49c4d" /></p>

## -R flag with chmod/chown/chgrp

First is the chgrp command I used from creating directory:
<p><img width="500" alt="image" src="https://github.com/user-attachments/assets/3ab8b8d6-fa7a-4855-bb6e-5526172f78b9" /></p>

Here is a screenshot of me using the chmod command:
<p><img width="500" alt="image" src="https://github.com/user-attachments/assets/99bc830d-b86e-42ac-8ef6-e0fe7c402fe5" /></p>

the chown command:
<p><img width="500" alt="Screenshot 2026-09-13 120333" src="https://github.com/user-attachments/assets/fada8d48-17e9-4b47-a07c-1a1625f36423" /></p>


## Sudo Access
Mallory is granted a sudo access using the command "sudo usermod -aG sudo" and I also tested Mallory's access using "sudo ls /root"
<p><img width="500" alt="Screenshot 2026-09-13 122954" src="https://github.com/user-attachments/assets/3966af7d-12a5-4f43-8102-69027a2e004d" /></p>
The use of sudo is allowing users or granting users accessibility to something not anyone can have access or control to.  That is why it is only given to the users that are trusted with almost full control into the system.

## Clean-up Task
Finally all the files were removed or cleaned-up, I used "sudo rm -r /home/shared" command for this task.
<img width="600" alt="Screenshot 2026-09-13 123145" src="https://github.com/user-attachments/assets/67f77b7e-dfe7-4fdc-8e3b-f9b5fbd523fd" />


# Reflection
## How do Linux permissions differ from Windows ACL? 
Linux permission uses more basic tried-based ownership system for the owner, group, and others. While Windows ACL uses more detailed permission, list-based system where individual and groups can have distinct rules.

## What’s the effect of chmod 770 vs 750? 
Ok so the chmod 770 gives the owner and also the group a read, write, and execute permissions, while on the other hand chmod 750 gives the owner the read, write, and execute permission, but the group only has read and execute.

## What is the risk of adding users to the sudo group? 
Adding users in the sudo group can give them access to perform admin actions and has the ability to change the information which is why it is risky, giving sudo access to a wrong person can really create a security risk.

## Why is it important to verify with `su` and `whoami`? 
I learned that using "su" helps allow to switch between users and "whoami" checks which user is currently being used. These commands will help verify that the permissions are working correctly for each user that is why it is important.
