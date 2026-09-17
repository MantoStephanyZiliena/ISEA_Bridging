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
I successfully downloaded in my EC2 instance the external pdf " http://...EECS-2009-28.pdf " given in our lab activity. I used the command called "wget".
<img width="700" alt="image" src="https://github.com/user-attachments/assets/e736dd12-1fe1-4849-a00b-6e8863799dcd" />

## PDF Accessible
First I copy the pdf using the command "sudo cp" and then I checked if it worked using "ls -l". I went to the browser and typed my public IP address with the pdf file name to check if I can open it and IT WORKED!
<img width="700" alt="image" src="https://github.com/user-attachments/assets/0df59e99-9b4a-468a-8ba6-d719cd17290c" />

## Link inserted in HTML Page
I open the index.html in the terminal and added an anchor tag at the body section of the html, I placed the link at the top right corner of the page and when I click the link, it went straight to the pdf file which is just like the screenshot above this.
<p><img width="700" alt="image" src="https://github.com/user-attachments/assets/7bf2767b-8097-4cc9-a98b-8ff5f8fd059d" /></p>


## Budget Monitoring
I successfully created the budget to help me be alerted about the spending over AWS.
<img width="700" alt="image" src="https://github.com/user-attachments/assets/b5d99fa0-e370-4b36-9bdc-609c6c057212" />


## Instance Terminated
