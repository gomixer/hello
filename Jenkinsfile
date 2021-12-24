pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                def root = tool type: 'go', name: 'Go 1.17.5'
                
                withEnv(["GOROOT=${root}", "PATH+GO=${root}/bin"]) {
                    sh 'go version'
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
