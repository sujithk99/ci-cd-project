pipeline {
    agent any

    parameters {
        string(
            name: 'IMAGE_TAG',
            defaultValue: 'latest',
            description: 'Docker Image Tag'
        )
    }

    stages {

        stage('Build') {
            steps {
                echo "Building image with tag: ${params.IMAGE_TAG}"
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying image: docker-pipeline-app:${params.IMAGE_TAG}"
            }
        }
    }
}