pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat 'echo Building application...'
                bat 'echo This is my build artifact > app.txt'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Testing application...'
            }
        }

    }

    post {
        success {
            archiveArtifacts artifacts: 'app.txt'
        }
    }
}
