pipeline {
    agent {
        dockerfile true
    }

    stages {
        stage('Build') {
            steps {
                sh 'dokcer build -t fe-test-docker .'
            }
        }
    }
}