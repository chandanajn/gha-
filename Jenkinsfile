pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/project/repo.git'
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