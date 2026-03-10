# 🚀 DevOps CI/CD Pipeline Project

![Docker](https://img.shields.io/badge/Docker-Containerization-blue)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Orchestration-blue)
![Jenkins](https://img.shields.io/badge/Jenkins-CI/CD-red)
![Python](https://img.shields.io/badge/Python-Flask-green)
![DevOps](https://img.shields.io/badge/DevOps-Automation-orange)

This project demonstrates a **complete DevOps CI/CD pipeline** that automates application build and deployment using modern DevOps tools.

The pipeline builds a **Flask web application**, containerizes it using **Docker**, and deploys it to **Kubernetes (Minikube)**.

---

# 📌 DevOps Architecture

```
Developer
   │
   ▼
GitHub Repository
   │
   ▼
Jenkins CI/CD Pipeline
   │
   ▼
Docker Build
   │
   ▼
Docker Container
   │
   ▼
Kubernetes Cluster (Minikube)
   │
   ▼
Flask Application
```

---

# 🛠 Technologies Used

* Python (Flask)
* Docker
* Jenkins
* Kubernetes (Minikube)
* Git & GitHub

---

# 📂 Project Structure

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

# 🐳 Build Docker Image

```bash
docker build -t flask-devops-app .
```

---

# ▶ Run Docker Container

```bash
docker run -p 5000:5000 flask-devops-app
```

Open in browser

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

1. Clone repository from GitHub
2. Build Docker image
3. Run Docker container
4. Deploy application to Kubernetes

Pipeline configuration is defined in the **Jenkinsfile**.

---

# 📸 Project Screenshots

(Add screenshots here)

Example:

```
docs/
   ├── jenkins-pipeline.png
   ├── docker-container.png
   └── kubernetes-pods.png
```

Then display them in README:

```
![Jenkins Pipeline](docs/jenkins-pipeline.png)
![Docker Container](docs/docker-container.png)
![Kubernetes Pods](docs/kubernetes-pods.png)
```

---

# 🚀 Future Improvements

* Push Docker images to Docker Hub
* Deploy application on AWS EC2
* Use Amazon EKS for Kubernetes cluster
* Add monitoring with Prometheus & Grafana

---

# 👨‍💻 Author

Stanley Bodige

DevOps | Cloud | Cybersecurity Enthusiast

GitHub:
https://github.com/Bodigestanley
