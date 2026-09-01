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

        stage('Deploy to Dev') {
            when {
                expression {
                    params.ENV == 'dev'
                }
            }
            steps {
                bat 'echo Deploying to DEV environment'
            }
        }

        stage('Deploy to Staging') {
            when {
                expression {
                    params.ENV == 'staging'
                }
            }
            steps {
                bat 'echo Deploying to STAGING environment'
            }
        }

        stage('Deploy to Prod') {
            when {
                expression {
                    params.ENV == 'prod'
                }
            }
            steps {
                bat 'echo Deploying to PRODUCTION environment'
            }
        }
    }
}
