pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/chandanajn/gha-'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t myapp .'
            }
        }

        stage('Push Docker Image') {
            steps {
                sh 'docker push myapp'
            }
        }
    }
}