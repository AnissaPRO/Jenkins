pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout your code from version control system (e.g., Git)
                git 'https://github.com/AnissaPRO/Jenkins.git'
            }
        }
        stage('Build') {
            steps {
               
                echo 'build'
            }
        }
        stage('Test') {
            steps {
                
                echo 'test'
            }
        }
        stage('Deploy') {
            steps {
                // Deploy your application (optional)
                 sh 'bash index.js'
            }
        }
    }

    post {
        success {
            // Actions to perform when pipeline succeeds
            echo 'Pipeline succeeded!'
        }
        failure {
            // Actions to perform when pipeline fails
            echo 'Pipeline failed!'
        }
    }
}