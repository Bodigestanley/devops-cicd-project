pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/Bodigestanley/devops-cicd-project.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t devops-app .'
            }
        }

        stage('Run Docker Container') {
            steps {
                bat 'docker run -d -p 5000:5000 devops-app'
            }
        }

    }
}