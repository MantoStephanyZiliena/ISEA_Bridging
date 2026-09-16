# 1b-1 Linux Services, SSH, Firewalls and Compression

## Apache Web Server
For this lab activity, I first installed the Apache in my terminal using the command "sudo apt install apache2" and test it in "127.0.0.1"
<p><img width="500" alt="Screenshot 2026-09-12 222900" src="https://github.com/user-attachments/assets/20a8c406-145b-44bf-b576-825829be2ea1" /></p>
<p>&nbsp;</p>

Next, I modified the index.html page of the Apache by changing the title of it and putting my nickname inside the body of the content.
<p><img width="500" alt="Screenshot 2026-09-12 224312" src="https://github.com/user-attachments/assets/5bb19245-7488-4700-9c99-00c3a1d801eb" /></p>
<p>&nbsp;</p>

## Cloning Virtual Machine
Cloning my first virtual machine to have a partner for this lab activity.
<img width="500" alt="Screenshot 2026-09-12 231117" src="https://github.com/user-attachments/assets/c8db4480-ec53-4ba0-b7db-d8b683529996" />
<p>&nbsp;</p>

First thing I did with my Main VM and Partner VM was, get botht the IP address using "ip a" and open each IP address in firefox to check the installed Apache.

Here is the first Apache from the main vm which I checked using the partner vm:
<img width="450" alt="Screenshot 2026-09-15 170554" src="https://github.com/user-attachments/assets/72828ae3-800f-4e5f-ae6d-7202d3eba1ba" />

Here is the Apache from the partner vm which I checked using the main one:
<img width="450" alt="Screenshot 2026-09-15 170825" src="https://github.com/user-attachments/assets/5c267f97-1497-4bf6-aa44-4b221aee7d5c" />



## Nmap
I scan each VMs port using the nmap.

first one using the partners IP:
<p><img width="450" alt="image" src="https://github.com/user-attachments/assets/43822f40-5e6f-4d73-a12b-7f6fa931bf60" /></p>

The other one using the main IP:
<p><img width="450" alt="image" src="https://github.com/user-attachments/assets/aacd3ab3-4ae2-4748-8f04-ed4737ce85b8" /></p>

I also tried removing the installed Apache, and basically when I used the nmap after removing, the port 80 is also gone from the lists of ports.


## UFW
Here I enable the UFW using the command "sudo ufw enable" this will display the ports 80 and 22 in both VM.

Main VM:
<p><img width="450" alt="Screenshot 2026-09-15 183601" src="https://github.com/user-attachments/assets/f35df630-0567-4076-b404-ba54e246a1e0" /></p>
Partner VM:
<p></p><img width="450" alt="Screenshot 2026-09-15 190226" src="https://github.com/user-attachments/assets/7cab6718-b306-4d03-8357-0c0228ce2e48" /></p>
<p>&nbsp;</p>

## SSH
I attempt the command "ssh [partner_IP]" and troubleshoot using the UFW rules.
Here is the result:
<img width="450" alt="Screenshot 2026-09-15 185506" src="https://github.com/user-attachments/assets/91b3daf5-45c0-45d0-be7f-488d6a053706" />

And then I created a new user in the partner vm and then tested logging in via SSH.
<img width="450" alt="Screenshot 2026-09-15 191402" src="https://github.com/user-attachments/assets/7df2063d-411c-4816-b185-e5559d0e71fe" />
<p>&nbsp;</p>

## Project Gutenberg
I downloaded the file called Gutenberg using the command called "wget"
<img width="450" alt="Screenshot 2026-09-13 103352" src="https://github.com/user-attachments/assets/70c41a01-c89c-4908-aaf4-dafd600eede2" />
<p>&nbsp;</p>

Next is I compress it with "bzip2 books.tar, decompress it with "bunzip2", and extract with "tar -xvf".

Compressing:
<p><img width="450" alt="Screenshot 2026-09-15 203824" src="https://github.com/user-attachments/assets/c7197c03-92db-4ac6-8cb9-fa02b4255c76" /></p>

Decompressing and extracting:
<p><img width="450" alt="image" src="https://github.com/user-attachments/assets/17a4b3a4-9605-4fc4-b437-5168a88fb232" /></p>

Confirms that the extraction worked:
<p><img width="450" alt="image" src="https://github.com/user-attachments/assets/5925d366-ca96-4062-8887-4a98e5f30961" /></p>
<p>&nbsp;</p>

# Challenge Activities

## Challenge 1: Remote File Creation via SSH
First I replace my main VM username into my partner VM username and IP.
<p><img width="450" alt="image" src="https://github.com/user-attachments/assets/312020c3-aa0e-4a4e-8fda-44f5b2c57e87" /></p>
Next I created a file called Hi_Partner using the "touch" command.
<p><img width="450" alt="image" src="https://github.com/user-attachments/assets/82afe48e-0e21-4fe4-8a1f-df082fd66ec7" /></p>

## Challenge 2: Remote GUI Apps
For this challenge I tried opening gedit over SSH and it did not work because SSH does not provide a graphical display.
But If I open it just through my terminal, it will work and it look like this:
<img width="450" alt="Screenshot 2026-09-15 214249" src="https://github.com/user-attachments/assets/fcd63bda-b0a3-451f-b84c-b822d805aef2" />


## Challenge 3: SCP File Transfer
For this Challenge I created I file in my main VM called Hi_Partner and send it to my partner VM.
<img width="450" alt="image" src="https://github.com/user-attachments/assets/e571253e-415a-405b-b3af-903fa276b6d3" />

This is what it looks like when I open the file inside the partner VM.
<img width="450" alt="image" src="https://github.com/user-attachments/assets/aa838263-3cc0-4019-ac23-c74d8145e135" />


## Challenge 4: Compress & Share Books
Last challenge, I created a books folder and downloaded books using "wget", created a tar archive, and compress it just like the first one I did.
<p><img width="450" alt="Screenshot 2026-09-15 222400" src="https://github.com/user-attachments/assets/5620f39b-9e18-4a5b-9a7a-200879c632d9" /></p>

And lastly, I transfer it to my partner VM.
<p><img width="450" alt="Screenshot 2026-09-15 222726" src="https://github.com/user-attachments/assets/84390828-ecc2-4bcb-bd47-5c91cc7c3603" /></p>

# Reflection

## What’s the role of a firewall in managing services? 
Firewall can control which networks connection is allowed to reach or leave a computer. When managing services, the firewall basically block unwanted access, allowing only the required services and reduce security risk. 

## How did SSH access deepen your understanding of Linux as a server? 
For me, SSH access deepen my understanding of Linux as a server because I can manage an operating system like Linux by just using a command line and it help me understand how I can manage, configure, and monitor a server.

## Why is file compression important in server contexts? 
Compressing files is important because it can help lessen the amount of storage needed to store and transfer files, this makes it more efficient to manage a server as well.

## How does user privilege management help secure systems?
User management can help secure a system by controlling user access and permissions, which can help prevent unuathorized users from having an access to the computers data or files.


