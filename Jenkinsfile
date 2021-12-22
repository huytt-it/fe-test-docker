pipeline {
    agent any

    stages {
        stage('Build docker image') {
           steps {
             sh 'docker build -t fe-test-docker -f Dockerfile .'
         }
        }
    }
}