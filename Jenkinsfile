pipeline {
    agent { dockerfile {
        filename 'fe-test-docker'
        label 'my-defined-label'
    } }

    stages {
        stage('Build docker') {
           steps {
             echo 'mvn clean install'
         }
        }
    }
}