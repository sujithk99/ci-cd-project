pipeline {
    agent any

    stages {

        stage('Parallel Validation') {
            parallel {

                stage('Unit Tests') {
                    steps {
                        echo 'Running Unit Tests'
                    }
                }

                stage('Security Scan') {
                    steps {
                        echo 'Running Security Scan'
                    }
                }
            }
        }

        stage('Build') {
            steps {
                echo 'Building Application'
            }
        }
    }
}