pipeline {
    agent any
    stages {
        stage('chkeckout '){
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'git-yomipounds', url: 'https://github.com/YomiPounds/test-shared.git']]])
            }
        }
        stage('first-stage'){
            steps {
                sh "echo I am a boy"
            }
        }
    }
}