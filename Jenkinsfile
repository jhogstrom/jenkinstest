pipeline {
    agent none
     stages {
            stage('Running in parallel'){
                parallel {
                    stage('Build .Net') {
                        agent {
                            docker { image 'mcr.microsoft.com/dotnet/sdk:6.0' }
                        }
                        steps {
                            echo 'Currently building the project on windows'
                            sh 'csc --version'
                        }
                    }
                    stage('Build Node') {
                        agent {
                            docker { image 'node:16.13.1-alpine' }
                        }
                        steps {
                            echo 'Currently building the project on linux'
                            sh 'node --version'
                        }
                    }
                }
        }
    }
}