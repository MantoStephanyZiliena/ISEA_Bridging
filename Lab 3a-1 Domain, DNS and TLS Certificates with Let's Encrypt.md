# 3a-1 Domain, DNS and TLS Certificates with Let's Encrypt

I launched a new instance on AWS since I terminated the last one. I named it ubuntu-lab, created a new key pair, 
and added https on the network setttings.
<p><img width="700" alt="image" src="https://github.com/user-attachments/assets/912a1be6-ea3a-4660-a518-b120331e743f" /></p>
<p>&nbsp;</p>

I installed the Apache web server again.
<img width="700" alt="Screenshot 2026-09-18 223837" src="https://github.com/user-attachments/assets/caf847dd-3b40-42d8-a7f8-4fa4c8bc8eb7" />
<p>&nbsp;</p>

I created a Duck DNS domain named stephanyweb.duckdns.org and register it to use my server's public IP address 
so it can be accessed using the domain name instead of the IP address.
<img width="700" alt="Screenshot 2026-09-18 231947" src="https://github.com/user-attachments/assets/821868ac-32c2-4d83-9a0c-6295ff93904d" />
<p>&nbsp;</p>

Here is what it looks like of my apache web page opened using my own domain name: http://stephanyweb.duckdns.org
<img width="700" alt="Screenshot 2026-09-18 232930" src="https://github.com/user-attachments/assets/9af1cfcc-9c60-448c-9d89-f07961b267ef" />
<p>&nbsp;</p>

# Reflection
## What is the role of DNS in Internet presence? 
DNS is basically a human readable domain name, and that name is being translated into an IP address which a computer can understand so that it can be open inside a web browser. Basically a DNS helps make it easy for people to remember an address with just a name not like with the normal IP address full of numbers.

## Why does DNS propagation take time? 
The DNS propagation takes time because DNS records are cached at so many servers around the world, that is why it takes time before it can actually check for updates.

## How does Let’s Encrypt validate domain ownership? 
The Let's Encrypt basically uses a protocol called ACME which confirm that you actually control the domain before giving certification for your own domain name. It will ask for a specific url to check if they can see it and they will give confirmation once they see it.

## What are the risks if TLS is not configured on a public-facing site? 
If TLS is not configured on a public-facing site, attackers can tamper with the data like the passwords and a lot more.
That is why it is important to configure TLS.

## What could happen if you leave your cloud VM running for months?
If a cloud VM is running for months, the user should already expect some charges from the cloud owner because every time a cloud VM is used, it starts running but after using it, it should also be stopped or terminated so that it wont charge because they will know that an instance is not in used or it is already terminated.
