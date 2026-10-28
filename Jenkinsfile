
        stage('Docker Run') {
            steps {
                sh '''
                    docker rm -f flask-container || true
                    docker run -d --name flask-container -p 5000:5000 ${IMAGE_NAME}:latest
                '''
            }
        }
