pipeline {
    agent any 
    stages {
        stage('Checkout') { 
            steps {
                sh 'echo checkout'
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/harveyjustin7/DevOpsPath']]])
            }
        }
        stage('Test') { 
            steps {
                sh 'echo test'
            }
        }
        stage('Deploy') { 
            steps {
                sh 'echo deploy'
            }
        }
    }
}
