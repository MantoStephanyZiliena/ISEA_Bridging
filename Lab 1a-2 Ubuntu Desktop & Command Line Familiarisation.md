# 1a-2 Ubuntu Desktop and Command Line Familiarisation
<p>&nbsp;</p>

## GUI Familiarisation
In this section, I familiarize myself with the GUI of Ubuntu by following the lab activities and exploring the desktop.
The following screenshots shows how I went through it.

First I went to Firefox and search Google just to check if the internet works in my Ubuntu.
<img width="600" alt="Screenshot 2026-09-12 211654" src="https://github.com/user-attachments/assets/06edb546-2a12-4cb7-97e1-d316219c3452" />
<p>&nbsp;</p>

Next I went to the App Center and decided to Install the LibreOffice Writer 
since it is not pre-installed on my Ubuntu, but in may differ, some Ubuntu have it already installed by default.
<img width="600" alt="Screenshot 2026-09-12 212636" src="https://github.com/user-attachments/assets/d303e9f6-801d-4af0-82ce-29e55a675fdd" />
<p>&nbsp;</p>

I opened the LibreOffice and tried typing on it just to check if it actually works. 
(Just notice that its the math one, I'll change this one later)
<p><img width="600" alt="Screenshot 2026-09-12 213108" src="https://github.com/user-attachments/assets/1ad53e86-c7c4-47c1-ac0e-3316f852b246" /></p>
<p>&nbsp;</p>

I also explored the file manager and navigate through the directory structure.
<img width="600" alt="Screenshot 2026-09-12 213231" src="https://github.com/user-attachments/assets/d6f27b10-c2e3-4ea1-9a63-538abd345300" />
<p>&nbsp;</p>

Lastly, I went to the terminal side by side with the file explorer just to see the changes real time
after I created a text file in the terminal using the touch command.
<img width="600" alt="Screenshot 2026-09-12 213907" src="https://github.com/user-attachments/assets/85abd615-5406-4e5d-8460-56127606859c" />
<p>&nbsp;</p>

## CLI Basics and Operations
For this section, I will be going through some basic commands and operations using the Ubuntu terminal.

First is I used the command "ps -e", this command will show all the running processes, and then used "top" to see all those processes real time showing the over all CPU usage. After that, I press 1 to show each CPU core used seperately and the screenshot below shows the real time processes and the two CPU used.
<img width="500" alt="Screenshot 2026-09-14 205725" src="https://github.com/user-attachments/assets/fc42b03c-c693-437b-b482-5897c6eeb3d3" />
<p>&nbsp;</p>

Next commands are "ls" and "ls -la", these two commands are used to show files in the file manager. The difference is that using ls would only show all the visible files and folders in the directory while the ls -la will show all files even the hidden files like .bashrc.
<p><img width="500" alt="Screenshot 2026-09-14 211321" src="https://github.com/user-attachments/assets/580f2ac5-3fed-428a-b620-d4cf7fe97295" /></p>
<p>&nbsp;</p>

I created a textfile using the touch command, after creating it I installed a command called "gedit" so I can open the textfile, and copy a few paragraphs from google and paste it inside the textfile. After that, I tried "nano" to open the textfile in the terminal itself, and below is the screenshot for it.
<img width="500" alt="image" src="https://github.com/user-attachments/assets/8e8cf7ed-403c-4acd-b84a-75b7695fae74" />
<p>&nbsp;</p>

Next are the commands called "cat" and "less". The cat command will show the whole textfile paragraph in the terminal while less will move to a scrollable file in terminal and need to exit once done.
<img width="500" alt="image" src="https://github.com/user-attachments/assets/5763b630-5c89-4191-95f9-fcfc521a3596" />
<p>&nbsp;</p>

For the next one, we have "cp" and "mv", they are use for copying and renaming a file. So what I did is I used cp to copy my textfile and named it textfile2, after that, I had the textfile2 be renamed as textfile3 using the command mv.
<img width="500" alt="Screenshot 2026-09-14 215535" src="https://github.com/user-attachments/assets/01424219-48cf-4591-ab82-23c64dd14df0" />
<p>&nbsp;</p>

Another command called "ls -lah" which also displays all the files from the file manager including the hidden files as well as the files sizes.
<p><img width="500" alt="image" src="https://github.com/user-attachments/assets/196c1555-9edd-485d-ab33-405be654fb8c" /></p>
<p>&nbsp;</p>

Now we have commands called "uname -a", "lsb_release -a" and "hostnamectl". These command are used to display the system information, Ubuntu distribution information, and last is the system identity information.
<img width="500" alt="image" src="https://github.com/user-attachments/assets/3e790b4a-3215-4447-82cd-0dec92910b0f" />
<p>&nbsp;</p>

Finally, we have the last command called "ls -alt" which is also similar to other ls commands but this one display the files sorted by the most recent modified first.
<p><img width="500" alt="image" src="https://github.com/user-attachments/assets/a2f84b8f-4c08-4cc9-a246-49c435142884" /></p>
<p>&nbsp;</p>

## Super User and Permissions
In this section, I learned that Super user is the root user in Linux. Basically the root user is the only one who has the permission to change something in the system and able create or add new user. The screenshot below is an example.
<img width="500" alt="image" src="https://github.com/user-attachments/assets/27a43d54-9931-4bbd-8ae4-91f950df1c94" />
<p>&nbsp;</p>

## Network Configuration and DNS
The goal in this section is to check the IP address and and test if VM can reach other devices.

First is I check my IP address using the command "ip a" and then I ping googles DNS and it worked.
<img width="500" alt="image" src="https://github.com/user-attachments/assets/b957501c-9a65-45b3-8e2a-840be9139f62" />
<p>&nbsp;</p>

Next is I added the Google's IP address and assigned it a local name, now it is easier to ping using the local name than remembering the IP address.
<p><img width="500" alt="Screenshot 2026-09-14 230913" src="https://github.com/user-attachments/assets/3d660d28-6f16-4e7f-a2bd-0df0184d088c" /></p>
<p>&nbsp;</p>

Now I used the "whois" command to look up informtion about the Google DNS.
<img width="500" alt="image" src="https://github.com/user-attachments/assets/7b5b54a2-fb3e-4990-9ec9-6323143b30bc" />
<p>&nbsp;</p>

Lastly, I checked my IP address using a website called "whatismyipaddress".
<img width="500" alt="Screenshot 2026-09-14 232755" src="https://github.com/user-attachments/assets/d91a8347-bc24-4317-be88-2a067a0bc527" />
<p>&nbsp;</p>

## System and Hardware Info
This section shows the hardware resources like processor, memory, and storage.

Here we can see all the details of the Ubuntu, also using the command "less /proc/cpuinfo" I was able to see all info regarding the CPU like how 2 processors are used to run the Ubuntu.
<img width="500" alt="image" src="https://github.com/user-attachments/assets/e0bb3066-8ae4-4e16-8fbc-ec488a8cd955" />
<p>&nbsp;</p>

For the last part, I tried turning the output into a file and also using commands like cat and less again to display the output in two different ways.
<p><img width="500" alt="image" src="https://github.com/user-attachments/assets/2d993f63-14ac-4e15-b68c-0644c3afa59e" /></p>
<p>&nbsp;</p>

## Software Installation
For this section, I try installing a software using the terminal.

Here I installed vlc using the terminal.
<p><img width="500" alt="image" src="https://github.com/user-attachments/assets/63d70ece-3a40-41ca-b526-e9575ddeccc4" /></p>
<p>&nbsp;</p>

## Reflection
Lab 1a-2 had taught me a lot, from CLI commands, super user and permission, to Network Configuration. It took me a long time to finish the lab but it was worth it because I learned a lot from it. I feel like I already have the grip of using the Ubuntu terminal from all the commands I had to try. Before doing this lab, I only knew how to open a terminal in ubuntu and that's it, so learning different kinds of commands for this lab felt a lot but understanding the use of all commands felt an accomplishment. So overall, through this lab, it made me more confident to navigate Linux for future labs activity and learn more from each one of it.






