pipeline {
    agent any

    stages {

        stage('Environment Info') {
            steps {
                bat 'echo Job Name: %JOB_NAME%'
                bat 'echo Build Number: %BUILD_NUMBER%'
                bat 'echo Workspace: %WORKSPACE%'
                bat 'echo Build URL: %BUILD_URL%'
            }
        }

        stage('Build') {
            steps {
                bat 'echo Building application...'
            }
        }

    }
}
