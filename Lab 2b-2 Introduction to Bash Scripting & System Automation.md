#  2b-2 Introduction to Bash Scripting & System Automation

## Part 1: Navigating the File System and Managing Files
For the first part, I used different kinds of command to create a directory, copy a file, rename, move a file, and remove it.
<p><img width="600" alt="Screenshot 2026-09-17 212134" src="https://github.com/user-attachments/assets/f867d20c-5729-4262-922f-db1e613543d6" /></p>

## Part 2: Creating and Executing Basic Bash Scripts
I created a basic bash script and execute it. I used "#!/bin/bash" to let ubuntu know which interpreter runs the script and that is Bash. I used the
string called "echo" and wrote something using the "$(whoami)" which is inside the echo.
<p><img width="600" alt="image" src="https://github.com/user-attachments/assets/483f4686-b933-45ab-8014-1e3ccfe89596" /></p>

## Part 3: Implementing Loops and Conditionals
This is the bash scripting code I created inside the file called system_info.sh. First I tried the Loop statement using the for and do loop, The system will loop 5 times because it is asked to count 5 times. Next is the Conditional statement using the if/elif/else statement, the conditional statement will asked the user to enter a number.
<img width="600" alt="image" src="https://github.com/user-attachments/assets/497d6075-2181-4f99-9d0a-66ad3dac5d4c" />

Loop Statement (for, do)
<p><img width="600" alt="image" src="https://github.com/user-attachments/assets/0a3a7f5f-7dae-4563-b663-451befa0a9df" /></p>

Conditional Statement (if/elif/else)
<p><img width="600" alt="Screenshot 2026-09-17 231233" src="https://github.com/user-attachments/assets/c4e41993-59d3-4e59-b22e-5ea40e384842" /></p>
<img width="600" alt="Screenshot 2026-09-17 231500" src="https://github.com/user-attachments/assets/f345075d-76dd-4ec2-8726-3561fa78be67" />

## Part 4: Automating System Monitoring Tasks 
<img width="600" alt="image" src="https://github.com/user-attachments/assets/af01d2a4-3900-4ec7-a895-a4c2c92ee956" />
<img width="600" alt="image" src="https://github.com/user-attachments/assets/776223f8-d882-4652-b499-5c3b4789d495" />
<img width="600" alt="Screenshot 2026-09-17 233805" src="https://github.com/user-attachments/assets/57661bfa-8d9f-46fd-aeba-020e85b67fe7" />

# Reflection
## What command did you use to create a new directory?
To create a new directory or folder, I used the command called "mkdir" which means make a directory. So just enter the command and add the name you want for the directory and then just enter its already gonna be inside the file management.

## How can you view the contents of a file without opening it in a GUI? 
I can open a file using a command called "cat" which helps view a file just inside the terminal itself. So just like the mkdir, you write the command followed by the file name then press enter and the text inside the file will appear in the terminal.

##  What is the purpose of `chmod 777`? 
The purpose of the command "chmod 777" which means change mode is basically having the user, a group, and others to have full access of read, write, and execute to a specific file.

## What does `#!/bin/bash` do at the start of a script? 
The command "#!/bin/bash" basically tells the system what kind of script should run in the terminal, and in that case, it should be the Bash. This command is also placed at the top of the script. 

## What happens when invalid input is entered into a script? 
When an invalid input is entered into a script, the may not work or show a error message telling that it is not valid input.
When this happen, we should always just try giving a valid input to make the script work.

## What output does `free -h` show? 
The command "free -h" will give an output of the information about the system memory, like the available, used, and total of the RAM being used.

## How would you monitor network bandwidth in a Bash script? 
To monitor the network bandwidth inside a bash script, I will use a commands like "ifstat" and "vnstat" which will help me monitor the network traffic and help me check how much data is being used.

