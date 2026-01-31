# Azure Linux VM Lab

This is my first basic cloud lab where I created a Linux virtual machine in Microsoft Azure. I am learning Azure, Linux, and cloud fundamentals, so this lab was mainly to understand how a virtual machine works and how to access it.

## VM Setup

I created a new resource group and then created an Ubuntu 22.04 virtual machine.  
For this lab I used the Standard D4s v3 size, which has 4 vCPUs and 16 GB RAM.  
Most of the settings were kept as default. I enabled SSH access to log in to the VM.  
Azure automatically created the virtual network, subnet, network interface, and public IP.

## Connecting to the VM

After the VM was created, I connected to it using SSH from my terminal:

ssh deva@<public-ip>

I entered my password and logged in successfully.

## Commands Used

After logging in, I ran these basic Linux commands to verify the system:

ip a # Check IP address
hostname # Check system hostname
lsb_release -a # Check OS version
df -h # Check disk usage
free -h # Check memory usage
lscpu # Check CPU information
sudo systemctl status ssh # Check SSH service status


## Observations

From these commands, I confirmed the following:

- The VM was running correctly  
- The OS was Ubuntu 22.04 LTS  
- The network interface was configured with a private IP  
- CPU, RAM, and disk storage were correctly allocated  
- SSH service was active and listening  

## Summary

This lab helped me understand the process of creating a Linux virtual machine on Azure, connecting to it using SSH, and checking basic system information.  
In future labs, I plan to install a web server and test hosting a simple application.
