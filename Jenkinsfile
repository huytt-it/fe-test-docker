pipeline {
    agent any

    stages {
        stage('Build docker') {
           steps {
             sh 'docker build -t fe-test-docker .'
         }
        }
    }
}