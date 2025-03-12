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
---

    ✅ 3. Update the System
sudo yum update -y

    ✅ 4. Install Apache Web Server
sudo yum install httpd -y

    ✅ 5. Start and Enable the Web Server
sudo systemctl start httpd
sudo systemctl enable httpd

    ✅ 6. Create and Deploy a Web Page
# Navigate to the web root directory
cd /var/www/html

# Create a simple index.html file
sudo nano index.html

<h1>Hello from Oladapo's Cloud Web Server!</h1>

     ✅ 7. View Your Live Page
http://18.227.114.52

💡 Skills Demonstrated
AWS EC2 provisioning
SSH and key-based access
Linux terminal navigation
Apache web server installation
Security Group configuration
HTML file deployment on a cloud server

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Oladapo's Cloud Web Server</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
      color: #333;
      text-align: center;
      padding-top: 100px;
    }
    h1 {
      color: #2c3e50;
    }
    p {
      font-size: 18px;
    }
  </style>
</head>
<body>
  <h1>Hello from Oladapo's Cloud Web Server!</h1>
  <p>This web page is hosted on an AWS EC2 instance using Apache.</p>
  <p>Project by <strong>Oladapo Adenekan</strong></p>
</body>
</html>

✍️ Author
Oladapo Adenekan
Cloud & DevOps Enthusiast
📍 Ohio, USA
LinkedIn- linkedin: www.linkedin.com/in/oladapo568


## ⭐ Summary

This hands-on project demonstrates my ability to launch and configure an AWS EC2 instance, establish secure SSH access using a key pair, install and manage a web server using Apache, and deploy a custom HTML page to the cloud.  

It showcases my foundational skills in cloud computing, Linux server management, networking (security groups), and basic web hosting.  

This project reflects the real-world tasks expected in entry-level cloud, DevOps, IT support, and cybersecurity roles — and is part of my continued learning journey toward cloud and GRC security excellence.













