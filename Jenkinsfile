pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/sujithk99/ci-cd-project.git'
            }
        }

        stage('Syntax Check') {
            steps {
                sh 'node --check index.js'
            }
        }
    }
}