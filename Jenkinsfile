
pipeline {
    agent any

    environment {
        IMAGE_NAME = 'henco8/flask-code-checkout'
    }

    stages {
        stage('Code Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/HenCo8/flask-code-checkout.git'

                sh 'ls -la'
            }
        }

        stage('Docker Build+Tag') {
            steps {
                sh 'docker build -t ${IMAGE_NAME}:latest .'
            }
        }
    }
}
