pipeline {
    agent any
    environment {
        DOCKERHUB_CREDENTIALS= credentials('pushDockerHub')
    }

    stages {
        stage('Login') {
           steps {
             sh 'echo $DOCKERHUB_CREDENTIALS_PSW | docker login -u $DOCKERHUB_CREDENTIALS_USR --password-stdin'
         }
        }
        stage('Logout') {
           steps {
             sh 'docker logout'
         }
        }
    }
}