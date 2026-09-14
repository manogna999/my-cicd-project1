pipeline {
    agent any

    stages {

        stage('Docker Check') {
            steps {
                bat '"C:\\Users\\manog\\AppData\\Local\\Programs\\DockerDesktop\\resources\\bin\\docker.exe" --version'
            }
        }

        stage('Docker Build') {
            steps {
                bat '"C:\\Users\\manog\\AppData\\Local\\Programs\\DockerDesktop\\resources\\bin\\docker.exe" build -t my-cicd-app:1.0 .'
            }
        }

        stage('Docker Images') {
            steps {
                bat '"C:\\Users\\manog\\AppData\\Local\\Programs\\DockerDesktop\\resources\\bin\\docker.exe" images'
            }
        }
    }
}