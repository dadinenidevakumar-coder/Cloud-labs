Azure Lab 2 - Linux VM Web Server (Nginx) Setup and Outputs
# Azure Lab 2 - Nginx Web Server

This is my second cloud lab.  
In this lab, I created a Linux VM in Microsoft Azure and installed a web server (Nginx).

## What I did
- Connected to my Azure VM using SSH
- Updated the system packages
- Installed Nginx
- Started and enabled the Nginx service
- Created a simple HTML page
- Checked that the web server is running

## Commands I used
sudo apt update -y
sudo apt upgrade -y
sudo apt install nginx -y
sudo systemctl start nginx
sudo systemctl enable nginx
echo "<h1>Welcome to Deva's Azure Web Server</h1>" | sudo tee /var/www/html/index.html

## Output file
All the lab outputs are saved in **Lab2-output.text**

## What I learned
- How to install software on a Linux VM
- How a web server works
- How to create a simple webpage on Azure VM
- How to save output files and upload to GitHub

