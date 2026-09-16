# 2b-1 Cloud Web Server Deployment with Amazon EC2

For this lab activity, we are task to sign in to Amazon Web Service and we will be configuring 
a virtual machine, install Apache web server, serve files online, and understand basic budgeting 
and cost management in cloud environments.

## EC2 Instance Launched and Running
For the first part, I was able to launch the AWS EC2 successfully
<img width="600" alt="Screenshot 2026-09-13 160116" src="https://github.com/user-attachments/assets/47d9c750-84ad-48fe-b332-a5017eaf37e0" />

Next I have it running and I already able to use it to run Linux commands on my Windows Powershell.
<img width="600" alt="Screenshot 2026-09-13 160538" src="https://github.com/user-attachments/assets/b9842b3a-de18-486c-9065-327dedd7e1ed" />

## Security Group
For the security group inbound rules is allowing SSH through port 22 and https through port 80.
<img width="600" alt="image" src="https://github.com/user-attachments/assets/3e75cbf3-f1ab-485d-ad00-4cdcce7695a4" />

## SSH Access Successfully
I connected to the AWS EC2 Ubuntu instance using SSH successfully. 
<img width="600" alt="image" src="https://github.com/user-attachments/assets/f3b82d7d-b734-4a05-b44e-dcf749673685" />

## Installed Apache
Using the command "sudo apt install apache2" on my powershell, I was able to install Apache on the same public IP I have for my AWS.
<p><img width="600" alt="Screenshot 2026-09-13 163118" src="https://github.com/user-attachments/assets/288c6136-64fc-4c43-a95d-2dd488f8d921" /></p>

## Custom index.html
I customized the index.html a bit. I just change the "it work!" into my name and I checked it using my public IP address and it worked.
<p><img width="600" alt="image" src="https://github.com/user-attachments/assets/437adbe9-c3db-44b4-978f-ebbaf8acb324" /></p>

## External File DL with wget

## PDF Accessible

## Link inserted in HTML Page

## Budget Monitoring

## Instance Terminated
