pipeline {
    agent any

    stages {
stage('Checkout Code') {
    steps {
        git branch: 'main',
        url: 'https://github.com/sujithk99/ci-cd-project.git'
    }
}        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run Application Test') {
            steps {
                sh 'node index.js'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t cicd-app .'
            }
        }
    }
}