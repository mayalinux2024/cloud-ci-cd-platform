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

- Flask App (Docker): [http://13.60.15.129:5000](http://13.60.15.129:5000)
- Latest Version: [http://13.60.15.129:8081](http://13.60.15.129:8081)


---

## 📸 Screenshots

### 1. GitHub Commit History
(Shows webhook-triggering commits)

<img width="823" height="473" alt="github-commits" src="https://github.com/user-attachments/assets/4a405d27-28b7-4833-86b0-f97f4f27b751" />


### 2. Jenkins Pipeline Success
(Build # showing successful execution)

<img width="417" height="430" alt="Jenkins-jobs-build" src="https://github.com/user-attachments/assets/6bb6735b-bc21-4758-be7b-7acb5f6b0127" />

### 3. Jenkins Console Output
(Docker build + deployment logs)

<img width="577" height="472" alt="Jenkins-build#9-console-1" src="https://github.com/user-attachments/assets/20db4ebc-ab86-4256-bae4-bba1bab6c94a" />

----

<img width="470" height="470" alt="Jenkins-build#9-console-2" src="https://github.com/user-attachments/assets/b1093be6-6993-478a-924d-7e74fb001eb4" />

----

<img width="466" height="467" alt="Jenkins-build#9-console-3" src="https://github.com/user-attachments/assets/818e45e0-0d61-4b24-bb58-449c5bbab044" />

----


### 4. Running Application
(Live Flask app in browser)

<img width="388" height="109" alt="port-5000-version-1" src="https://github.com/user-attachments/assets/04ef2d43-5fbd-4ec3-afdc-eaffdf7eb989" />

<img width="407" height="72" alt="port-8081-version-2" src="https://github.com/user-attachments/assets/6c179eb4-acea-4a2c-8a93-8c649e6cb96d" />

<img width="398" height="67" alt="port-8081-version-3-webhook-build" src="https://github.com/user-attachments/assets/1953c352-55fe-411f-88bd-bac892fb7f36" />

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
