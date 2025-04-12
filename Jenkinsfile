pipeline {
    agent any  // Runs on any available agent (node)
    stages {
        stage('Checkout') {
            steps {
                echo 'Cloning code from GitHub...'
                git branch: 'main', url: 'https://github.com/mukulKanitkar/devops_assignment1.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the project for devops assignment'
            }
        }
        stage('Test') {
            steps {
                echo 'Running testst for devops assignment'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Deploying code to Staging Environment'
            }
        }
        
        stage('Deploy to Production') {
            steps {
                echo 'Deploying code to Production Environment'
            }
        }
    }
    post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check logs!'
        }
    }
}