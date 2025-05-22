pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm  // This checks out your GitHub code
            }
        }
        
        stage('Build') {
            steps {
                echo 'Building the application...'
                // Add your build commands here, for example:
                // sh 'mvn clean package'  // For Java projects
                // sh 'npm install'       // For Node.js projects
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add your test commands here
            }
        }
    }
    
    post {
        always {
            echo 'Pipeline completed - cleaning up'
        }
    }
}
