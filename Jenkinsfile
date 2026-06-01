pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/sujithk99/ci-cd-project.git'
            }
        }

        stage('Lint Validation') {
            steps {
                echo 'Lint Stage Executed Successfully'
            }
        }

        stage('Pipeline Validation') {
            steps {
                sh 'echo Multiple Commit Test Passed'
            }
        }
    }
}