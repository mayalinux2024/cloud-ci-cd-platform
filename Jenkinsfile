pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/mayalinux2024/cloud-ci-cd-platform.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t flask-app .'
            }
        }

        stage('Stop Old Container (if running)') {
            steps {
                sh 'docker stop flask-app || true'
                sh 'docker rm flask-app || true'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 8081:5000 --name flask-app flask-app'
            }
        }
    }
}
