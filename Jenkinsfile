pipeline {
    agent any

    stages {
        stage('Check Docker') {
            steps {
                sh 'which docker || echo Docker_Not_Found'
                sh 'docker --version || true'
            }
        }
    }
}