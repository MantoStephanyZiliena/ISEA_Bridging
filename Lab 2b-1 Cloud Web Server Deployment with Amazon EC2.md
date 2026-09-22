# 2b-1 Cloud Web Server Deployment with Amazon EC2

For this lab activity, we are tasked to sign in to Amazon Web Service and we will be configuring 
a virtual machine, install Apache web server, serve files online, and understand basic budgeting 
and cost management in cloud environments.
<p>&nbsp;</p>

## EC2 Instance Launched and Running
For the first part, I was able to launch the AWS EC2 successfully
<img width="700" alt="Screenshot 2026-09-13 160116" src="https://github.com/user-attachments/assets/47d9c750-84ad-48fe-b332-a5017eaf37e0" />

Next I have it running and I already able to use it to run Linux commands on it.
<img width="700" alt="Screenshot 2026-09-13 160538" src="https://github.com/user-attachments/assets/b9842b3a-de18-486c-9065-327dedd7e1ed" />
<p>&nbsp;</p>

## Security Group
For the security group inbound rules is allowing SSH through port 22 and https through port 80.
<img width="700" alt="image" src="https://github.com/user-attachments/assets/3e75cbf3-f1ab-485d-ad00-4cdcce7695a4" />
<p>&nbsp;</p>

## SSH Access Successfully
I connected to the AWS EC2 Ubuntu instance using SSH successfully. 
<img width="700" alt="image" src="https://github.com/user-attachments/assets/f3b82d7d-b734-4a05-b44e-dcf749673685" />
<p>&nbsp;</p>

## Installed Apache
Using the command "sudo apt install apache2" on my powershell, I was able to install Apache on the same public IP I have for my AWS.
<p><img width="700" alt="Screenshot 2026-09-13 163118" src="https://github.com/user-attachments/assets/288c6136-64fc-4c43-a95d-2dd488f8d921" /></p>
<p>&nbsp;</p>

## Custom index.html
I customized the index.html a bit. I just change the "it work!" into my name and I checked it using my public IP address and it worked.
<p><img width="700" alt="image" src="https://github.com/user-attachments/assets/437adbe9-c3db-44b4-978f-ebbaf8acb324" /></p>
<p>&nbsp;</p>

## External File DL with wget
I successfully downloaded in my EC2 instance the external pdf " http://...EECS-2009-28.pdf " given in our lab activity. I used the command called "wget".
<p><img width="700" alt="image" src="https://github.com/user-attachments/assets/e736dd12-1fe1-4849-a00b-6e8863799dcd" /></p>
<p>&nbsp;</p>

## PDF Accessible
First I copy the pdf using the command "sudo cp" and then I checked if it worked using "ls -l". I went to the browser and typed my public IP address with the pdf file name to check if I can open it and IT WORKED!
<img width="700" alt="image" src="https://github.com/user-attachments/assets/0df59e99-9b4a-468a-8ba6-d719cd17290c" />
<p>&nbsp;</p>

## Link inserted in HTML Page
I open the index.html in the terminal and added an anchor tag at the body section of the html, I placed the link at the top right corner of the page and when I click the link, it went straight to the pdf file which is just like the screenshot above this.
<p><img width="700" alt="image" src="https://github.com/user-attachments/assets/7bf2767b-8097-4cc9-a98b-8ff5f8fd059d" /></p>
<p>&nbsp;</p>

## Budget Monitoring
I successfully created the budget to help me be alerted about the spending over AWS.
<img width="700" alt="image" src="https://github.com/user-attachments/assets/b5d99fa0-e370-4b36-9bdc-609c6c057212" />
<p>&nbsp;</p>

## Terminate Instance
Last step I did for this activity after the challenges was to terminate my Instance in AWS for clean up. I will just be creating a new instance for other future lab activities.
<p><img width="700" alt="image" src="https://github.com/user-attachments/assets/c18dc668-f40e-4668-9a31-62439461d415" /></p>
<p>&nbsp;</p>

# Challenges

## Challenge 1: Network Latency Testing
For this challenge, I tried to compare two servers in different countries. I tried to ping Google.com which is used in US and compare it to Google.com.ph which is used in the Philippines. I noticed that both server has the same time in milliseconds which is 4007ms or 4 seconds, this just tell me that they both don't have any delays.
<img width="700" alt="image" src="https://github.com/user-attachments/assets/efd96524-2e94-4bc1-b2ed-6f028bbfdd21" />

## Challenge 2: Create a Custom HTML Page
I successfully created my custom html page in my EC2 web server and here is the output. It is a simple html structure without any CSS style on it.
<p><img width="700" alt="image" src="https://github.com/user-attachments/assets/28b8a77d-e8b7-4757-9510-85b4a32ea969" /></p>

# Reflection
## What were the benefits of cloud deployment over local virtualisation?
  
For me, cloud deployment like AWS is easier to use. It was easy log in, create an instance, and connect to EC2 terminal to do some commands. I can also manage my web server anywhere which is convenient.

## How does Apache serve files, and how did you verify this?
  
 Apache is a web server that receives http or https requests and that request is send to web browser. In my case, I installed apache2 on my EC2 terminal and open it to my web browser to verify it if it worked.

 ## What did you learn about file ownership and permissions?
  
I learned that Linux files has owners, groups, and other which can get permission to read, write, and execute a file.
Using a command "chmod 777" which means change mode to give a full read, write, and execute to anyone which is the owner, a group, and the others.

 ## What risks are associated with leaving instances running?
  
Leaving an instance running even if we are done doing our work, can leave us some unexpected charges, that is why it is important to stop our instance after using it or after running it because it can also cause a risk into the open server we  leave running.

## How would you explain the difference between DNS and /etc/hosts to a client?
  
I would explain that DNS basically turns domain name into IP addresses using some naming system, while the /etc/host also does something similar but it use local file on computer to map names into IP addresses, For me, using a DNS is better for websites so that many people can access it much easier.  

 

