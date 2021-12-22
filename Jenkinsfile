pipeline {
    agent { dockerfile true }

    stages {
        stage('Build dokcer') {
           steps {
             echo 'mvn clean install'
         }
        }
    }
}