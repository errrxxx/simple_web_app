pipeline {
    agent any
    stages {
        // Stage 1: Initialize
        stage('Build with Maven') {
            steps {
                echo 'Builduing with Maven...'
            }
        }
        // Stage 2: Build
        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'mvn install'
            }
        }
        // Stage 3: Deploy
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
            }
        }
    }
    post {
        always {
            echo 'Pipeline completed!'
        }
    }
}
