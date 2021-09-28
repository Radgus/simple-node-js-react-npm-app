pipeline {
    agent {
        docker {
            image 'node:lts-buster-slim' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Install dependencies') { 
            steps {
                sh 'npm i' 
            }
        }
        stage('test') {
            steps {
                sh 'npm run test'
            }
        }
    }
}