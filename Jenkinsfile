pipeline {
    agent { 
        label 'node14'
    } 
    tools {
        nodejs 'nodejs14'
    }
    stages {
        stage('Install') {
            steps {
                sh '''
                    npm install -f
                '''
            }
        }
        stage('Build') {
            steps {
                sh '''
                    npm run build
                '''
            }
        }
    }
}