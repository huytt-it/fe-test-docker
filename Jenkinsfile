pipeline {
    agent any
    environment {
        DOCKERHUB_CREDENTIALS= credentials('pushDockerHub')
    }

    stages {
         stage('Build image') {
           steps {
             sh 'docker build -t fe-test-docker .'
         }
        }

        stage('Login') {
           steps {
             sh 'echo $DOCKERHUB_CREDENTIALS_PSW | docker login -u $DOCKERHUB_CREDENTIALS_USR --password-stdin'
         }
        }

        stage('Push') {
           steps {
             sh 'docker push huytt26/testjenkin:latest'
         }
        }

        post {
           always {
             sh 'docker logout'
         }
        }
    }
}