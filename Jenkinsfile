pipeline {
    agent any
    environment {
        DOCKERCREDENTIAL= credentials('dockerHubAdmin')
    }

    stages {
        stage('Login') {
           steps {
             sh 'echo $DOCKERCREDENTIAL | docker login -u $DOCKERCREDENTIAL --password-stdin'
         }
        }
    }
}