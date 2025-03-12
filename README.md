# 🚀 AWS EC2 Web Server Project

This project demonstrates how I launched and configured an EC2 instance on AWS, connected via SSH, installed Apache, and deployed a basic web page using **Amazon Linux 2023**.

---

## 📸 Screenshots

- ✅ EC2 instance running:  
  ![EC2 Running](./EC2-instance-running.png)

- 🔐 SSH connection to instance:  
  ![SSH Access](./EC2_SSH_Connection.PNG)

- 🌍 Web server running:  
  ![Web Server](./Setup_Web_Server_on_Ec2.PNG)

---

## 📌 Overview

This project showcases my ability to:

- Launch an EC2 instance on AWS
- Set up secure access using SSH and key pairs
- Install and configure an Apache web server
- Deploy and view a live HTML web page
- Use Linux commands to manage the server

---

## 🔧 Step-by-Step Instructions

### ✅ 1. Launch an EC2 Instance
- Region: `us-east-2 (Ohio)`
- AMI: **Amazon Linux 2023**
- Instance type: `t2.micro` (Free Tier eligible)
- Created new key pair: `oladapo-key.pem`
- Configured **Security Group** to allow:
  - **SSH (port 22)** – for terminal access
  - **HTTP (port 80)** – to view the website

---

### ✅ 2. Connect to Instance via SSH

```bash
# Move into Downloads where .pem file is saved
cd /mnt/c/Users/YourUsername/Downloads

# Set permissions on the key file
chmod 400 oladapo-key.pem

# Connect to EC2
ssh -i oladapo-key.pem ec2-user@18.227.114.52
