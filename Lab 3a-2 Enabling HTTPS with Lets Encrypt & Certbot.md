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
<img width="700" alt="image" src="https://github.com/user-attachments/assets/d48b8ad3-4952-4101-9b53-4ce0be721051" />
<p>&nbsp;</p>

Lastly, I tried doing the certbot renew --dry-run to try renewing my certification and it worked successfully.
<img width="700" alt="Screenshot 2026-09-19 112227" src="https://github.com/user-attachments/assets/09b59ad7-0eac-4859-9839-0ad97d1e5adb" />
<p>&nbsp;</p>

# Reflection
- Why is HTTPS important for modern web applications? 

- What entity issued your site’s TLS certificate? 

- How long is your certificate valid for, and how can it be renewed? 

- What happens if a certificate expires and is not renewed? 

- Why does Let’s Encrypt require port 80 or 443 to be open for verification? 


