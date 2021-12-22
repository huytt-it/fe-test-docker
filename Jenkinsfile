pipeline {
    agent { dockerfile {
        additionalBuildArgs  '--build-arg version=1.0.2'
    }

    stages {
        stage('Build docker') {
           steps {
             echo 'mvn clean install'
         }
        }
    }
}