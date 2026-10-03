pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                sh 'go build'
                echo 'Build completed successfully'd'
            }
        }

        stage('Test') {
            steps {
                sh 'go test ./...'
            }
        }
    }
}
