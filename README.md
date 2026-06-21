# 🚀 CI/CD Pipeline Project using Jenkins, Docker, and GitHub

## 📌 Project Overview

This project demonstrates a complete **CI/CD pipeline** using Jenkins, GitHub, and Docker on AWS EC2.

Every code change pushed to GitHub automatically triggers a Jenkins pipeline that builds, deploys, and runs a Dockerized Flask application.

---

## 🏗️ Architecture
GitHub (Source Code)
↓
GitHub Webhook
↓
Jenkins CI Server (EC2)
↓
Docker Build
↓
Docker Container Deployment
↓
Flask Application (Live)


---

## ⚙️ Tech Stack

- Jenkins (CI/CD Automation)
- Docker (Containerization)
- GitHub Webhooks (Trigger system)
- Flask (Python Web App)
- AWS EC2 (Deployment Server)
- Linux Ubuntu

---

## 📁 Project Structure
cloud-ci-cd-platform/
├── app/
│ └── app.py
├── Dockerfile
├── Jenkinsfile
├── requirements.txt


---

## 🔄 CI/CD Pipeline Stages

Jenkins pipeline performs the following steps:

1. **Checkout Code** from GitHub
2. **Build Docker Image**
3. **Stop Existing Container (if running)**
4. **Remove Old Container**
5. **Run New Docker Container**
6. **Deploy Flask Application**

---

## 🔗 Webhook Integration

GitHub Webhooks automatically trigger Jenkins builds on every push to the main branch.

---

## 🌐 Live Application

- Flask App (Docker):  
  `http://13.60.15.129:5000`

- Latest Deployment:  
  `http://13.60.15.129:8081`

---

## 📸 Screenshots

### 1. GitHub Commit History
(Shows webhook-triggering commits)

### 2. Jenkins Pipeline Success
(Build # showing successful execution)

### 3. Jenkins Console Output
(Docker build + deployment logs)

### 4. Running Application
(Live Flask app in browser)

---

## 🎯 Key Features

- Fully automated CI/CD pipeline
- GitHub → Jenkins integration via webhook
- Dockerized application deployment
- Zero manual deployment after setup
- Real-world DevOps workflow simulation

---

## 🧠 What I Learned

- CI/CD pipeline design
- Jenkins job configuration
- Docker container lifecycle
- GitHub webhook automation
- AWS EC2 deployment
- Linux server management

---

## 📌 Author

Maya Elfeky

Built as a DevOps learning project to demonstrate end-to-end CI/CD automation.
