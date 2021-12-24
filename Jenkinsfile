pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
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
