pipeline {
    agent any

    parameters {
        choice(
            name: 'ENV',
            choices: ['dev', 'staging', 'prod'],
            description: 'Select deployment environment'
        )
    }

    stages {

        stage('Build') {
            steps {
                bat 'echo Building application...'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Testing application...'
            }
        }

        stage('Deploy') {
            steps {
                bat 'echo Deploying application to %ENV% environment...'
            }
        }

    }
}
