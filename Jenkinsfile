pipeline {
    agent any

    stages {

        stage('Check Python Version') {
            steps {
                sh 'python3 --version'
            }
        }

        stage('Run Python Script') {
            steps {
                sh 'python3 hello.py'
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