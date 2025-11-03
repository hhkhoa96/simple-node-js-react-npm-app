pipeline {
    agent any

    tools {
        nodejs 'NodeJS'
    }

    stages {
        stage('Info') {
            steps {
                sh '''
                    node --version
                    npm --version
                '''
            }
        }

        stage('Build') { 
            steps {
                sh '''
                    ls -la
                    npm install
                    npm run build
                    ls -la
                '''
            }
        }
    }
}