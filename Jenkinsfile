pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building project...'
                bat 'echo Build successful'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'echo Tests successful'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}