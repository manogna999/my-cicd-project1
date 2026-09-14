pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building application...'
                bat 'dir'
            }
        }

       stage('Test') {
            steps {
                bat 'if exist hello.txt (echo TEST PASSED) else (echo TEST FAILED & exit /b 1)'
            }
        } 
        
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }

    post {
        success {
            echo 'CI/CD pipeline completed successfully!'
        }

        failure {
            echo 'CI/CD pipeline failed!'
        }
    }
}