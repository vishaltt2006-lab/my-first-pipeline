pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Source code is available'
            }
        }

        stage('Test') {
            steps {
                sh 'test -s index.html'
                echo 'Basic test passed'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t my-first-app:1.0 .'
            }
        }
    }
}
