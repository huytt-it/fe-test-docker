pipeline {
    agent any
    environment {
        DOCKERHUB_CREDENTIALS= credentials('myDockerHub')
    }

    stages {
        stage('Login') {
           steps {
             sh 'echo $DOCKERHUB_CREDENTIALS_PSW | docker login -u $DOCKERHUB_CREDENTIALS_USR --password-stdin'
         }
        }
    }
}