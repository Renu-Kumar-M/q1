pipeline {
    agent any 
    stages {
        stage('Checkout Code') {
            steps {
                // Clones the source code from your GitHub repository configuration
                checkout scm
            }
        }
        stage('Build') {
            steps {
                // Runs the simple Python program
                sh 'python3 app.py'
            }
        }
    }
}
