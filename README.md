# 🚀 AWS CI/CD Deployment using GitHub Actions, Docker, Amazon ECR & EC2

A simple Full Stack web application deployed automatically using a complete CI/CD pipeline on AWS.

## 📌 Project Overview

This project demonstrates an automated deployment pipeline using:

- GitHub
- GitHub Actions
- Docker
- Amazon Elastic Container Registry (ECR)
- Amazon EC2
- Nginx

Whenever code is pushed to the **main** branch, GitHub Actions automatically:

1. Builds a Docker image.
2. Pushes the image to Amazon ECR.
3. Connects to the EC2 instance using SSH.
4. Pulls the latest Docker image.
5. Runs the updated container automatically.

---

# 🏗️ Architecture

```
Developer
     │
     ▼
GitHub Repository
     │
     ▼
GitHub Actions
     │
     ▼
Docker Build
     │
     ▼
Amazon ECR
     │
     ▼
Amazon EC2
     │
     ▼
Docker Container
     │
     ▼
Live Website
```

---

# 📂 Project Structure

```
aws-deploy/
│
├── .github/
│   └── workflows/
│       └── aws-deploy.yml
│
├── Dockerfile
├── index.html
└── README.md
```

---

# 🛠️ Technologies Used

- HTML
- CSS
- JavaScript
- Docker
- Git
- GitHub
- GitHub Actions
- AWS EC2
- Amazon ECR
- Nginx

---

# ⚙️ CI/CD Workflow

### Step 1
Developer pushes code to GitHub.

### Step 2
GitHub Actions starts automatically.

### Step 3
Docker image is built.

### Step 4
Image is pushed to Amazon ECR.

### Step 5
GitHub Actions connects to EC2 through SSH.

### Step 6
EC2 pulls the latest Docker image.

### Step 7
Old container is removed.

### Step 8
New Docker container starts.

---

# 🐳 Docker

Build Image

```bash
docker build -t aws-deploy .
```

Run Container

```bash
docker run -d -p 80:80 aws-deploy
```

---

# ☁️ AWS Services Used

- Amazon EC2
- Amazon ECR
- IAM
- GitHub Actions

---

# 📷 Project Output

The application is successfully deployed on an Amazon EC2 instance and can be accessed through the EC2 Public IPv4 address.

Example:

```
http://<EC2_PUBLIC_IP>
```

---

# 🔄 GitHub Actions Workflow

The workflow automatically executes whenever changes are pushed to the **main** branch.

Main stages include:

- Checkout Source Code
- Configure AWS Credentials
- Login to Amazon ECR
- Build Docker Image
- Push Docker Image
- Connect to EC2
- Pull Latest Image
- Deploy Docker Container

---

# 📋 Prerequisites

- AWS Account
- EC2 Instance
- Amazon ECR Repository
- IAM User
- Docker Installed
- Git Installed
- GitHub Repository

---

# 👨‍💻 Author

**PASUPATHY RAM P**

DevOps | AWS | Docker | GitHub Actions | Full Stack Development

---

# ⭐ Features

- Automated CI/CD Pipeline
- Dockerized Application
- Zero Manual Deployment
- Cloud Deployment on AWS
- Version Control using Git
- Easy to Scale
- Secure Deployment using GitHub Secrets

---

## 📜 License

This project is created for educational.