pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout your code from version control system (e.g., Git)
                git 'https://github.com/AnissaPRO/Jenkins'
            }
        }
        stage('Build') {
            steps {
                // Build your project (e.g., Maven, Gradle)
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                // Run your tests (e.g., JUnit, Selenium)
                sh 'mvn test'
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