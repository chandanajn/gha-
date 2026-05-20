pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t jnchandana/gha:latest .'
            }
        }

        stage('Push Docker Image') {
            steps {
                bat 'docker push jnchandana/gha:latest'
            }
        }
    }
}