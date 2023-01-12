pipeline {
    agent {
        docker { image 'node:16.13.1-alpine' }
    }
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello, Maven'
            }
        }
        stage('Example Test') {
            steps {
                echo 'Hello, JDK'
            }
        }
    }
}