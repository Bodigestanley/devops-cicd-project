# 🚀 DevOps CI/CD Pipeline Project

This project demonstrates a **complete DevOps CI/CD pipeline** that automates application build and deployment using modern DevOps tools.

The pipeline builds a **Flask web application**, containerizes it using **Docker**, and deploys it to **Kubernetes (Minikube)**.

---

## 📌 Project Architecture

Developer → GitHub → Jenkins → Docker → Kubernetes → Application

1️⃣ Developer pushes code to GitHub
2️⃣ Jenkins automatically triggers the pipeline
3️⃣ Jenkins builds the Docker image
4️⃣ Docker container is created
5️⃣ Kubernetes deploys the container
6️⃣ Service exposes the application

---

## 🛠 Technologies Used

* Python (Flask)
* Docker
* Jenkins
* Kubernetes (Minikube)
* Git & GitHub

---

## 📂 Project Structure

```
devops-cicd-project
│
├── app.py
├── Dockerfile
├── Jenkinsfile
├── deployment.yaml
├── service.yaml
└── README.md
```

---

# ⚙️ Setup Instructions

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/Bodigestanley/devops-cicd-project.git
cd devops-cicd-project
```

---

## 🐳 Build Docker Image

```bash
docker build -t flask-devops-app .
```

---

## ▶ Run Docker Container

```bash
docker run -p 5000:5000 flask-devops-app
```

Open in browser:

```
http://localhost:5000
```

---

# ☸ Kubernetes Deployment

Start Minikube

```bash
minikube start
```

Deploy application

```bash
kubectl apply -f deployment.yaml
```

Create service

```bash
kubectl apply -f service.yaml
```

Check running pods

```bash
kubectl get pods
```

Check services

```bash
kubectl get services
```

Open application

```bash
minikube service flask-service
```

---

# 🔄 Jenkins CI/CD Pipeline

The Jenkins pipeline performs the following stages:

1️⃣ Clone repository from GitHub
2️⃣ Build Docker image
3️⃣ Run container
4️⃣ Deploy to Kubernetes cluster

Pipeline is defined inside the **Jenkinsfile**.

---

# 👨‍💻 Author

Stanley Bodige
DevOps | Cloud | Cybersecurity Enthusiast

GitHub:
https://github.com/Bodigestanley
