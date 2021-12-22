pipeline {
    agent { dockerfile {
        filename 'fe-test-docker'
     } 
    }

    stages {
        stage('Build docker') {
           steps {
             echo 'mvn clean install'
         }
        }
    }
}