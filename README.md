# DevOps CI/CD Pipeline Project

This project demonstrates a complete CI/CD pipeline using Jenkins, Docker, and GitHub to automatically build and deploy a Python Flask application.

## 🚀 Technologies Used

- GitHub
- Jenkins
- Docker
- Python
- Flask

## 📂 Project Structure

devops-cicd-project/
│
├── app.py
├── Dockerfile
├── Jenkinsfile
└── README.md

## ⚙️ CI/CD Pipeline Workflow

1. Code is pushed to GitHub
2. Jenkins automatically triggers the pipeline
3. Jenkins builds the Docker image
4. Docker container runs the application
5. Application is exposed on port 5000

Pipeline Flow:

GitHub → Jenkins → Docker Build → Docker Container → Application Running

## 🐳 Docker Commands Used

Build Image

docker build -t devops-app .

Run Container

docker run -d -p 5000:5000 devops-app

Check Running Containers

docker ps

## 🌐 Application Access

Open browser:

http://localhost:5000

## 📊 Future Improvements

- Push Docker image to Docker Hub
- Deploy application to Kubernetes
- Deploy infrastructure on AWS
- Add monitoring using Prometheus and Grafana

## 👨‍💻 Author

Stanley Bodige
