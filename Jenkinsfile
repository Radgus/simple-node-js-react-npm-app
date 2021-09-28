pipeline {
    agent any
    tools {
        nodejs '11.1.0'
    }

    options {
        timeout(time: 5, unit: 'MINUTES')
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