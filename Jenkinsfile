pipeline {
    agent any

    tools {
        nodejs 'nodejs-14' // 'nodejs-14' is the Node.js installation label/version
    }

    stages {
        stage('Build') {
            steps {
                script {
                    // Assuming you have Node.js installed on your Jenkins server
                    sh 'npm install'
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    // Assuming you have a deployment script or command
                    // For simplicity, we're just restarting the app here
                    sh 'npm start > /dev/null 2>&1 &'
                }
            }
        }
    }
}
