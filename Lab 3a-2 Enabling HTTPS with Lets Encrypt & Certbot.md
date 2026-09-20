# 3a-2 Enabling HTTPS with Lets Encrypt & Certbot

For this lab activity, I first had my own DNS using the DuckDNS which is free and easy to use. 
I then configure it so that I can open my installed apache in my Ubuntu to my domain name. 
Http is used to open my domain in my web browser and this is how it looked like:
<p><img width="700" alt="Screenshot 2026-09-18 232930" src="https://github.com/user-attachments/assets/37b66aa5-d96a-4e74-8050-e9af507ef721" /></p>
As you can see from the screenshot, the domain name is basically not secure yet so that is what the lab is all about, 
Installing a certbot and having my domain name a certification to also enable https.
<p>&nbsp;</p>

Using my EC2 instance terminal, I installed the certbot using the command called "sudo apt install".
<img width="700" alt="Screenshot 2026-09-19 111346" src="https://github.com/user-attachments/assets/ef8e470c-8c52-4d1e-9d01-f351cd39f4ac" />
<p>&nbsp;</p>

Next is the screenshot of my successful certification using Let's Encrpyt.
<img width="700" alt="Screenshot 2026-09-19 112136" src="https://github.com/user-attachments/assets/a8d28470-6661-471a-bf21-2794f6291216" />
<p>&nbsp;</p>

 Here is my apache web page using my domain name in https which means that my connection is secure and my certificate is valid.
<p><img width="700" alt="image" src="https://github.com/user-attachments/assets/d48b8ad3-4952-4101-9b53-4ce0be721051" /></p>
<p>&nbsp;</p>

Lastly, I tried doing the certbot renew --dry-run to try renewing my certification and it worked successfully.
<img width="700" alt="Screenshot 2026-09-19 112227" src="https://github.com/user-attachments/assets/09b59ad7-0eac-4859-9839-0ad97d1e5adb" />
<p>&nbsp;</p>

# Reflection
## Why is HTTPS important for modern web applications? 
For me, https is important for modern web application because from the word itself, Hyper Text Transfer Secure, which means a web application connection is being secure. It basically encrypts data and protects all important information, it also https is now required to make sure that a web application is trusted.

## What entity issued your site’s TLS certificate? 
The Let's Encrypt is the site that issued my TLS certification which is a free and automated certification authority, it was also easy to do and had it really fast so that my domain name can be used using https.

## How long is your certificate valid for, and how can it be renewed? 
The Let's Encrypt certificate lasts for 90 days, and I can renew it using a command called "certbot renew", I can use that command inside my EC2 terminal. I tried a dry run on how to renew and it was an easy process.

## What happens if a certificate expires and is not renewed? 
Basically if a certificate expires and is not renewed, the browser will show security warnings or might also block access. That is why it is not important to renew a certificate.

## Why does Let’s Encrypt require port 80 or 443 to be open for verification? 
It requires port 80 or 443 because the domain validation work with those ports. It basically wants it to reach server the same way a real user or visitor would. And we also know that port 80 and port 443 are like the main ports used for web servers and more.

