# Secure VPC Design for a Public-Facing Application

## 📌 Project Overview
This project demonstrates a secure AWS VPC architecture for a public-facing application using AWS best practices.

The design removes direct internet access from application servers and databases while maintaining high availability and security.

---

## 🧠 Problem Statement
A startup hosted its backend EC2 instances and database directly on the internet, creating security risks such as:
- Open inbound access
- Publicly accessible database
- Increased attack surface

---

## 🎯 Solution
The architecture was redesigned to include:
- A custom VPC
- Public and private subnets
- Application Load Balancer (internet-facing)
- Private EC2 application servers
- Private RDS database
- NAT Gateway for controlled outbound internet access
- Least-privilege Security Groups

---

## 🏗 Architecture Diagram

![Secure VPC Architecture](architecture/secure-vpc-architecture.png)

---

## 🔐 Security Best Practices Applied
- Only the Load Balancer is internet-facing
- EC2 instances have no public IPs
- Database is in a private subnet
- Security Groups allow traffic only where required
- NAT Gateway controls outbound traffic

---

## 🧰 AWS Services Used
- Amazon VPC
- Amazon EC2
- Application Load Balancer
- Amazon RDS
- NAT Gateway
- Internet Gateway
- Security Groups
- Route Tables

---

## 🚀 Future Improvements
- Auto Scaling Group
- HTTPS using ACM
- AWS WAF integration
- CloudWatch monitoring

---

## 👤 Author
**Hope Ebeli**  
Aspiring Cloud Engineer
