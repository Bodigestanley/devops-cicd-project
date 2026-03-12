# 🚀 Kubernetes Microservices Deployment Project

![Docker](https://img.shields.io/badge/Docker-Containerization-blue)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Orchestration-blue)
![Minikube](https://img.shields.io/badge/Minikube-LocalCluster-yellowgreen)
![Python](https://img.shields.io/badge/Python-Flask-green)
![DevOps](https://img.shields.io/badge/DevOps-Automation-orange)

This project demonstrates a **complete Kubernetes microservices architecture** that deploys multiple containerized Flask applications and orchestrates them using **Kubernetes (Minikube)**.

The architecture consists of **4 microservices**:

* **Auth Service** – Handles authentication
* **Product Service** – Manages products
* **Order Service** – Handles orders
* **Frontend Service** – Provides the UI

---

# 📌 Microservices Architecture

```
           User
            │
            ▼
     Frontend Service
      ┌─────┴─────┐
      │           │
  Auth Service  Product Service
                  │
                  ▼
              Order Service
```

![Architecture Diagram](./screenshots/architecture.png)

---

# 🛠 Technologies Used

* Python (Flask)
* Docker
* Kubernetes (Minikube)
* Git & GitHub

---

# 📂 Project Structure

```
kubernetes-microservices-project
│
├── auth-service/
│   ├── app.py
│   └── Dockerfile
├── product-service/
│   ├── app.py
│   └── Dockerfile
├── order-service/
│   ├── app.py
│   └── Dockerfile
├── frontend/
│   ├── app.py
│   └── Dockerfile
├── kubernetes/
│   ├── auth-deployment.yaml
│   ├── product-deployment.yaml
│   ├── order-deployment.yaml
│   ├── frontend-deployment.yaml
│   └── ingress.yaml
├── screenshots/
│   ├── architecture.png
│   ├── auth-service.png
│   ├── product-service.png
│   ├── order-service.png
│   └── frontend-service.png
└── README.md
```

---

# ⚙️ Setup Instructions

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/Bodigestanley/kubernetes-microservices-deployment.git
cd kubernetes-microservices-deployment
```

---

# 🐳 Build Docker Images

```bash
docker build -t auth-service ./auth-service
docker build -t product-service ./product-service
docker build -t order-service ./order-service
docker build -t frontend-service ./frontend
```

---

# ▶ Load Images into Minikube

```bash
minikube image load auth-service:latest
minikube image load product-service:latest
minikube image load order-service:latest
minikube image load frontend-service:latest
```

---

# ☸ Kubernetes Deployment

Start Minikube:

```bash
minikube start
```

Deploy services:

```bash
kubectl apply -f kubernetes/
```

Check running pods:

```bash
kubectl get pods
```

Check services:

```bash
kubectl get services
```

Open Frontend service:

```bash
minikube service frontend-service
```

---

# 🔄 Microservices Overview

Each microservice runs as a separate containerized Flask application managed by Kubernetes. Deployments ensure replication, and services provide network access. Ingress routes requests to the correct service.

---

# 📸 Project Screenshots

![Auth Service](./screenshots/auth-service.png)
![Product Service](./screenshots/product-service.png)
![Order Service](./screenshots/order-service.png)
![Frontend Service](./screenshots/frontend-service.png)

---

# 🚀 Future Improvements

* Push Docker images to Docker Hub
* Deploy services on AWS EC2
* Use Amazon EKS for Kubernetes cluster
* Add monitoring with Prometheus & Grafana

---

# 👨‍💻 Author

Stanley Bodige

DevOps | Cloud | Cybersecurity Enthusiast

GitHub:
[https://github.com/Bodigestanley](https://github.com/Bodigestanley)
