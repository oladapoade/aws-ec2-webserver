# 🚀 EC2 Instance Web Server Project

This project demonstrates how I launched, configured, and connected to an AWS EC2 instance, and hosted a simple web page from the cloud using **Amazon Linux 2023**.

---

## 📌 Project Overview

I set up a cloud-based virtual server using AWS EC2, connected via SSH using a private key, and configured a basic web server to display a custom message.

---

## 🔧 Steps Performed

### 1. **Launched EC2 Instance**
- Region: `us-east-2 (Ohio)`
- OS: **Amazon Linux 2023**
- Instance type: `t2.micro`
- Created a new key pair (`oladapo-key.pem`)
- Opened necessary ports (port **22** for SSH, **80** for HTTP) via **security groups**

### 2. **Connected via SSH**
- Used terminal and `.pem` file for a secure SSH connection
- Set appropriate file permissions using `chmod 400 oladapo-key.pem`
- Connected using the command:

```bash
ssh -i oladapo-key.pem ec2-user@18.227.114.52

