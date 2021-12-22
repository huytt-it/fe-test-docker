pipeline {
    agent { dockerfile {
        additionalBuildArgs  'fe-test'
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