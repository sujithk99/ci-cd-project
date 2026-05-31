pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/sujithk99/ci-cd-project.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t docker-pipeline-app .'
            }
        }
    }
}