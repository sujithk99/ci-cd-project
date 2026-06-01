pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                echo 'Code Checked Out'
            }
        }

        stage('Build') {
            steps {
                echo 'Build Successful'
            }
        }

        stage('Test') {
            steps {
                echo 'Tests Passed'
            }
        }

        stage('Deploy Dev') {
            steps {
                echo 'Application Deployed to DEV'
            }
        }

        stage('Manual Approval') {
            steps {
                input 'Approve deployment to Staging?'
            }
        }

        stage('Deploy Staging') {
            steps {
                echo 'Application Deployed to STAGING'
            }
        }

        stage('Deploy Production') {
            steps {
                echo 'Application Deployed to PRODUCTION'
            }
        }
    }
}