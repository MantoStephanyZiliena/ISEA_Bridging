# 3a-1 Domain, DNS and TLS Certificates with Let's Encrypt

I launched a new instance on AWS since I terminated the last one. I named it ubuntu-lab, created a new key pair, 
and added https on the network setttings.
<img width="700" alt="image" src="https://github.com/user-attachments/assets/912a1be6-ea3a-4660-a518-b120331e743f" />

I installed the Apache web server again.
<img width="700" alt="Screenshot 2026-09-18 223837" src="https://github.com/user-attachments/assets/caf847dd-3b40-42d8-a7f8-4fa4c8bc8eb7" />

I created a Duck DNS domain named stephanyweb.duckdns.org and register it to use my server's public IP address 
so it can be accessed using the domain name instead of the IP address.
<img width="700" alt="Screenshot 2026-09-18 231947" src="https://github.com/user-attachments/assets/821868ac-32c2-4d83-9a0c-6295ff93904d" />

Here is what it looks like of my apache web page opened using my own domain name: http://stephanyweb.duckdns.org
<img width="700" alt="Screenshot 2026-09-18 232930" src="https://github.com/user-attachments/assets/9af1cfcc-9c60-448c-9d89-f07961b267ef" />
