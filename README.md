# aws-auto-scaling-load-balancer-docker
Aws first project
# 🚀 Scalable Web Application on AWS using Docker, Auto Scaling & Load Balancer

This project demonstrates how a Dockerized web application can be deployed on AWS using a scalable and fault-tolerant architecture.

The application is hosted on multiple EC2 instances managed by an Auto Scaling Group and traffic is distributed using an Application Load Balancer.

Refreshing the application shows different EC2 hostnames, proving that load balancing is working correctly.

---

## 🧠 What This Project Demonstrates

- Dockerizing an application for consistent deployment
- Hosting containers on Amazon EC2
- Auto Scaling Group for high availability
- Application Load Balancer for traffic distribution
- Real-world cloud debugging and setup

---

## 🛠️ Technologies Used

- AWS EC2
- Auto Scaling Group
- Application Load Balancer (ALB)
- Docker
- Amazon Linux
- Python (Flask)
- Docker Hub (public image registry)

---

## 📐 Architecture Overview

User
↓
Application Load Balancer
↓
Auto Scaling Group (EC2 Instances)
↓
Docker Container (Web Application)

---

## 📸 Proof of Work

- Auto Scaling Group showing running instances
- Load Balancer with healthy targets
- Application video showing hostname change on refresh

> Screenshots and demo video are available in the `screenshots/` folder.

---

## 🧪 How the Application Works

- The web app displays the hostname of the EC2 instance serving the request
- Each EC2 instance runs the same Docker container
- Refreshing the page routes traffic to different instances via the Load Balancer

This confirms:
- Load Balancer is working
- Auto Scaling is managing instances
- Application is running consistently across servers

---

## ▶️ How to Run Locally (Optional)

```bash
docker build -t traffic-app .
docker run -p 5000:5000 traffic-app
