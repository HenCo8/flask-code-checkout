
pipeline {
    agent any

    stages {
        stage('Code Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/HenCo8/flask-code-checkout.git'

                sh 'ls -la'
            }
        }
    }
}
