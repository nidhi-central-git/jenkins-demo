pipeline {
    agent any

    environment {
        APP_NAME = 'myapp'
        ENV = 'dev'
    }

    stages {

        stage('Show Environment') {
            steps {
                bat 'echo Application: %APP_NAME%'
                bat 'echo Environment: %ENV%'
            }
        }

        stage('Build') {
            steps {
                bat 'echo Building %APP_NAME% for %ENV% environment...'
            }
        }

    }
}
