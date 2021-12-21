pipeline {
    agent any

    stages {
        stage('Docker-build') {
            steps {
                sh 'docker buid -t fe-test-docker .'
            }
        }
    }
}