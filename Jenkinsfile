pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                script {
                    // Étape de construction
                    echo 'Building...'
                    
                }
            }
        }
        
        stage('Test') {
            steps {
                script {
                    // Étape de test
                    echo 'Testing...'
                   
                }
            }
        }
        
        stage('Deploy') {
            steps {
                script {
                    // Étape de déploiement
                    echo 'Deploying...'
                    sh 'node index.js'  // Lancement de l'application
                }
            }
        }
    }
}
