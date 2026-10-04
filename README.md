# AWS Application Load Balancer - Load Balancing Demo

## 📌 Project Overview

This project demonstrates how an AWS Application Load Balancer
distributes HTTP traffic across multiple EC2 instances running
Apache web servers.

## 🏗️ Architecture

Internet
   |
   v
Application Load Balancer
   |
   +----------------+
   |                |
   v                v
EC2 Server 1     EC2 Server 2
Apache           Apache

## ☁️ AWS Services Used

- Amazon EC2
- Application Load Balancer
- Target Group
- Security Groups
- Amazon Linux
- Apache HTTP Server

## 🛠️ Technologies

- HTML
- CSS
- Linux
- Apache
- AWS

## ⚙️ Implementation

### 1. EC2 Instances

Created two Amazon Linux EC2 instances.

### 2. Apache

Installed and configured Apache on both instances.

### 3. Web Pages

Created different HTML pages on each server to identify
which EC2 instance handled the request.

### 4. Target Group

Created an HTTP target group on port 80 and registered
both EC2 instances.

### 5. Application Load Balancer

Created an internet-facing Application Load Balancer
with an HTTP listener on port 80.

### 6. Health Checks

Configured HTTP health checks using `/`.

Both EC2 instances successfully became healthy targets.

## 🧪 Testing

Accessed the Application Load Balancer DNS name and verified
that requests were served by both EC2 instances.

## 📸 Screenshots

Screenshots are available in the `screenshots` directory.

## 📚 What I Learned

- Launching and configuring EC2
- Installing Apache on Linux
- Configuring Security Groups
- Creating Target Groups
- Configuring Application Load Balancers
- Understanding health checks
- Understanding traffic distribution
- Basic AWS networking concepts

## 🚀 Future Improvements

- Add Auto Scaling Group
- Add HTTPS using ACM
- Add Amazon S3 for static assets
- Add monitoring using CloudWatch
