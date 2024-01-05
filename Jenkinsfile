pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // Assuming you have Node.js installed on your Jenkins server
                    sh 'npm install'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    // Add your test commands here if needed
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    // Assuming you have a deployment script or command
                    // For simplicity, we're just restarting the app here
                    sh 'npm start'
                }
            }
        }
    }
}
