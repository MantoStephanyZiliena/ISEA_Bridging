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
<img width="500" alt="Screenshot 2026-09-13 101134" src="https://github.com/user-attachments/assets/d69c4112-39c9-44e1-85e3-b3010483217b" />
<p>&nbsp;</p>

## SSH
<img width="500" alt="Screenshot 2026-09-13 101958" src="https://github.com/user-attachments/assets/42d6cde0-e124-4572-a461-f5eac5de5922" />
<p>&nbsp;</p>
