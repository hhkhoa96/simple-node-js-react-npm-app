pipeline {
    agent any

    stages {
        agent {
            docker {
                image 'node:18-alpine'
                reuseNode true
            }
        }

        stage('Build') { 
            steps {
                sh '''
                    ls -la
                    node --version
                    npm --version
                    npm install
                    ls -la
                '''
            }
        }
    }
}