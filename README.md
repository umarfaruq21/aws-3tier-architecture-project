# 🚀 AWS 3-Tier Architecture Deployment Project

![Project Status](https://img.shields.io/badge/status-completed-brightgreen)
![Cloud](https://img.shields.io/badge/cloud-AWS-orange)
![Focus](https://img.shields.io/badge/focus-Cloud%20%26%20DevOps-blue)
![Project](https://img.shields.io/badge/project-3Tier%20Architecture-success)

---

# 📌 Project Overview

This project demonstrates the design and deployment of a production-style AWS 3-tier cloud architecture using EC2, VPC, public/private subnets, route tables, internet gateways, and security groups.

The project was built as part of my Cloud & DevOps learning journey to gain hands-on experience with real-world cloud infrastructure concepts.

---

# 📑 Table of Contents

- Architecture Overview
- Technologies Used
- EC2 Web Server Deployment
- VPC Setup
- Security Implementation
- Architecture Design
- Project Screenshots
- Key Learnings
- Resume Impact
- Future Improvements

---

# 🏗 Architecture Overview

```text
Users
   ↓
Internet Gateway
   ↓
Public Subnet
   ↓
EC2 Web Server
   ↓
Private Subnet
   ↓
Application Layer
   ↓
Database Layer (Port 3306 Restricted)
```

---

# 🔧 Technologies Used

- AWS EC2
- Amazon VPC
- Public & Private Subnets
- Security Groups
- Route Tables
- Internet Gateway
- Linux (Amazon Linux 2)
- Apache Web Server
- Git & GitHub

---

# 🌐 EC2 Web Server Deployment

## 📌 Overview

Launched and configured an EC2 instance to host a static website using Apache Web Server.

---

## ⚙️ EC2 Configuration

- Instance Type: t2.micro
- Operating System: Amazon Linux 2
- Public IP: Enabled
- Web Server: Apache (httpd)

---

## 🔐 Security Group Configuration

| Type | Port | Access |
|---|---|---|
| SSH | 22 | My IP |
| HTTP | 80 | Anywhere |

---

## 🛠 Commands Used

```bash
sudo yum update -y
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
```

---

## 🌍 Sample Web Page

```bash
echo "<h1>Welcome Umar Cloud Project 🚀</h1>" | sudo tee /var/www/html/index.html
```

---

# 🌐 VPC Setup

## 📌 Overview

Created a custom Virtual Private Cloud (VPC) to simulate a real-world cloud network architecture.

---

## ⚙️ VPC Configuration

| Component | CIDR |
|---|---|
| VPC | 10.0.0.0/16 |
| Public Subnet | 10.0.1.0/24 |
| Private Subnet | 10.0.2.0/24 |

---

## 🔧 Components Configured

- Internet Gateway attached to VPC
- Route Table configured for public subnet
- Public internet access enabled
- Subnet segmentation implemented

---

# 🔐 Security Implementation

## 📌 Security Group Design

| Layer | Security Group | Allowed Access |
|---|---|---|
| Web Layer | Web-SG | HTTP (80), SSH (22) |
| App Layer | App-SG | Internal Traffic Only |
| Database Layer | DB-SG | MySQL 3306 from App-SG |

---

## 🔒 Security Features

- Public and private subnet separation
- Layered security group access control
- Database access restricted internally
- Internet access limited to web layer

---

# 🏗 AWS 3-Tier Architecture Design

## 📌 Architecture Flow

```text
Users
   ↓
Web Server (Public Subnet)
   ↓
Application Layer (Private Subnet)
   ↓
Database Layer (Port 3306 Restricted)
```

---

# 📸 Project Screenshots

## 🏗 Architecture Diagram

<img width="1373" height="915" alt="1-architecture-diagram" src="https://github.com/user-attachments/assets/68e1acbe-a449-4a7b-9f44-e07038513ff4" />

---

## 🌐 EC2 Web Server

<img width="1920" height="751" alt="02-ec2-web-server" src="https://github.com/user-attachments/assets/251e742a-4e38-422b-91a3-543fe74d5735" />
---

## 🌍 VPC and Subnets

<img width="1901" height="782" alt="03-vpc-public-private-subnets" src="https://github.com/user-attachments/assets/c76b1072-3bcd-420d-bfc3-21d3db3a9030" />

---

## 🔐 Security Groups

<img width="814" height="210" alt="04 1-security-group-rules" src="https://github.com/user-attachments/assets/3f66a9c9-6c0b-4e83-96d7-bf54474c40f9" />
<img width="820" height="238" alt="04-security-group-rules" src="https://github.com/user-attachments/assets/28428944-f38e-4cd6-8155-a803aebe5507" />


---

## 🗺 Route Table Configuration

<img width="833" height="268" alt="05-route-table-configuration" src="https://github.com/user-attachments/assets/094a5834-e841-4d15-ad77-68e55caf7844" />

---
## 🌍 Website Output

<img width="931" height="401" alt="06-website-output" src="https://github.com/user-attachments/assets/42be64e1-9890-4f74-adcb-cf2ed4f723bb" />


---
# 📚 Key Learnings

- AWS cloud architecture fundamentals
- EC2 instance deployment
- VPC networking concepts
- Public and private subnet design
- Route table configuration
- Security group implementation
- Linux server administration
- Infrastructure planning and documentation

---

# 💼 Resume Impact

This project demonstrates:

- AWS cloud infrastructure setup
- Networking and subnet architecture
- Security implementation using Security Groups
- Linux administration skills
- Web server deployment
- Cloud architecture documentation
- GitHub project management

---

# 💡 Skills Demonstrated

- Amazon Web Services (AWS)
- Amazon EC2
- Amazon VPC
- Linux Administration
- Networking
- Security Groups
- Cloud Computing
- Infrastructure Deployment
- GitHub
- DevOps Fundamentals

---

# 🚀 Future Improvements

- Docker container deployment
- CI/CD pipeline using GitHub Actions
- AWS Load Balancer integration
- CloudWatch monitoring setup
- Terraform Infrastructure as Code
- Kubernetes deployment

---

# 🎯 Final Outcome

Successfully designed and documented a real-world AWS 3-tier architecture project suitable for Cloud & DevOps portfolio showcase.

This project helped strengthen my understanding of cloud networking, infrastructure security, and AWS deployment concepts.

---

# 👨‍💻 Author

Mahammad Umar Faruq Shaik

🔗 GitHub:
https://github.com/umarfaruq21/aws-3tier-architecture-project

🔗 LinkedIn:
https://www.linkedin.com/in/umarfaruqshaik/

---
✨ This project marks an important step in my Cloud & DevOps journey.
