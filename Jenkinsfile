pipeline {
    agent any

    parameters {
        choice(
            name: 'IMAGE_TAG',
            choices: ['latest', 'v1.0', 'v1.1'],
            description: 'Select Docker Image Version'
        )
    }

    stages {
        stage('Build') {
            steps {
                echo "Selected Image Tag: ${params.IMAGE_TAG}"
            }
        }
    }
}