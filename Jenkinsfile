
pipeline {
    agent any

    parameters {
        string(
            name: 'NAME',
            defaultValue: 'Daniel',
            description: 'Enter your name'
        )
    }

    stages {
        stage('Greeting') {
            steps {
                echo "Hello ${params.NAME}!"
            }
        }
    }
}
