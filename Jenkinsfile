pipeline {
    agent any

    stages {

        stage('Check Python Version') {
            steps {
                bat '"C:\\Users\\siran\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe" --version'
            }
        }

        stage('Run Python Script') {
            steps {
                bat '"C:\\Users\\siran\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe" hello.py'
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