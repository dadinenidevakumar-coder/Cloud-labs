Azure Linux VM Lab
 
This is my first basic cloud lab where I created a Linux virtual machine in Microsoft Azure. I am learning Azure, Linux and cloud fundamentals, so this lab was mainly to understand how a VM works and how to access it.

I created a new resource group and then created an Ubuntu 22.04 virtual machine. I used the D4s v3 size which has 4 vCPUs and 16GB RAM. I kept all settings mostly default except enabling SSH access. Azure also created a virtual network, subnet, public IP and network interface automatically.

After the VM finished creating, I connected to it using SSH from my terminal like this:
ssh deva@<public-ip>

I entered my password and logged in successfully. After logging in, I ran a few basic Linux commands to check the system.

Commands I used:
ip a            - to see IP address
hostname        - to see the system hostname
lsb_release -a  - to check OS version
df -h           - to check disk space
free -h         - to check memory
lscpu           - to see CPU information
systemctl status ssh - to check SSH service

From these commands, I confirmed that:
- the VM was running correctly
- network interface was configured
- OS was Ubuntu 22.04
- CPU, RAM and disk were showing properly
- SSH service was active

This lab helped me understand the basic process of creating a VM in Azure and connecting to it. I also practiced simple Linux commands. In the next labs, I plan to install a web server and try hosting a simple page.

This lab helped me understand the process of creating a Linux virtual machine on Azure, connecting to it using SSH, and checking basic system information.  
In future labs, I plan to install a web server and test hosting a simple application.
