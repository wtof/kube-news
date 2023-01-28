pipeline {
    agent any
    stages {
        stage('Build Docker Image') {
            steps {
                dockerapp = docker.build("wtof/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
            }
        }
    }
}