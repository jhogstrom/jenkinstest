pipeline {
    agent {
        docker { image 'node:16.13.1-alpine' }
    }
     stages {
        stage('Build') {
            steps {
                echo 'Currently building the project'
                sh 'node --version'
            }
        }
        stage('Test') {
            steps {
                echo 'Currently testing the project'
            }
        }
    }
}