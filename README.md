# Rise-Internship-Project-1
# AWS EC2 Static Website Deployment

## Project Overview

This project demonstrates how to deploy a static website on a cloud server using **Amazon EC2**. The purpose of this project is to understand the basic concepts of cloud hosting, Linux server management, and web server configuration as part of my **Cloud & DevOps internship learning**.

In this project, a Linux-based EC2 instance is launched, a web server is installed, and a static HTML/CSS website is hosted and made accessible through the internet.

---

## Cloud Platform

The cloud infrastructure used in this project is **Amazon Web Services (AWS)**.

---

## Project Objectives

The main objectives of this project are:

- Launch and configure an EC2 virtual machine
- Connect to the instance securely using SSH
- Install and configure an Apache web server
- Deploy a static HTML/CSS website
- Make the website publicly accessible using the EC2 public IP

---

## Technologies Used

- **AWS EC2 (Amazon Linux 2023)**
- **Linux Command Line**
- **Apache Web Server**
- **HTML5**
- **CSS3**
- **Git & GitHub**

---

## Project Architecture

User → Internet → AWS EC2 Instance → Apache Web Server → Static Website

---

## Implementation Steps

### 1. Launch EC2 Instance

- Logged into the AWS Management Console
- Created a new EC2 instance
- Selected **Amazon Linux 2023 AMI**
- Configured security group rules to allow:
  - **SSH (Port 22)**
  - **HTTP (Port 80)**

---

### 2. Connect to EC2 Instance

Connected to the server using SSH with the key pair.

```bash
ssh -i mykey.pem ec2-user@<Public-IP>
```

---

### 3. Install Apache Web Server

Updated the system and installed the Apache HTTP server.

```bash
sudo dnf update -y
sudo dnf install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
```

---

### 4. Deploy Website Files

Navigate to the Apache web directory and create the HTML file.

```bash
cd /var/www/html
sudo nano index.html
```

Add your HTML code for the website landing page.

---

### 5. Access the Hosted Website

Open the website in a browser using the EC2 public IP address:

```
http://<Public-IP>
```

---

## Project Outcome

The static website was successfully deployed on an AWS EC2 instance and made accessible over the internet through the public IP address.

---

## Key Learnings

Through this project, I learned:

- Basics of cloud computing using AWS
- How to launch and manage EC2 instances
- Connecting to Linux servers using SSH
- Installing and configuring Apache web servers
- Hosting static websites on cloud infrastructure
- Managing AWS security groups and network access

---

## Screenshots

![Image](https://github.com/user-attachments/assets/160901f7-f25b-4687-bd35-821f580546fe)
<br><br>
![Image](https://github.com/user-attachments/assets/f9d853b3-fd08-4456-878b-e9f83b60a673)
<br><br>
![Image](https://github.com/user-attachments/assets/fa912f36-6293-4875-a970-9558e25a59bc)
<br><br>
![Image](https://github.com/user-attachments/assets/8885bd38-44af-4329-a44f-204d3c1a0d91)
