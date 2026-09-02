pipeline {
    agent any 
    stages {
        stage('Checkout Code') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                // Changing 'sh' to 'bat' fixes the Windows execution error
                bat 'python sum.py'
            }
        }
    }
}
