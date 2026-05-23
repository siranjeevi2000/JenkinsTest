pipeline {
    agent any

    stages {

        stage('Check Python Version') {
            steps {
                bat 'python3 --version'
            }
        }

        stage('Run Python Script') {
            steps {
                bat 'python3 hello.py'
            }
        }

    }

    post {
        success {
            echo 'Pipeline executed successfully'
        }

        failure {
            echo 'Pipeline failed'
        }
    }
}