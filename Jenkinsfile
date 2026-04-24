pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps { checkout scm }
        }
        stage('Build') {
            steps { echo Building feature... }

        }
        stage('Test') {
            steps { sh 'echo Testing...' }
        }
        stage('Deploy') {
            steps { sh 'echo Deploying...' }
        }
    }
    post {
        always { echo 'Pipeline completed' }
        success { echo 'Success!' }
        failure { echo 'Failed!' }
    }
}

