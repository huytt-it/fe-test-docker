pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'dokcer build -t fe-test-docker .'
            }
        }
    }
}