pipeline {
    agent any

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
                bat 'echo Deploying application...'
            }
        }
    }

    post {
        success {
            bat 'echo Pipeline completed successfully!'
        }

        failure {
            bat 'echo Pipeline FAILED!'
        }

        always {
            bat 'echo Pipeline execution finished.'
        }
    }
}
