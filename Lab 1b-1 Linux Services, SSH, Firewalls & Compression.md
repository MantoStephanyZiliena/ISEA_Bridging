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



