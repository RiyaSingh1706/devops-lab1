pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/RiyaSingh1706/devops-lab1.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the project...'
                bat 'python --versionn'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'python app.py'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}