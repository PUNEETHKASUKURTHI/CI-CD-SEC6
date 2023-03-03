pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/PUNEETHKASUKURTHI/CI-CD-SEC6', credentialsId: '<CREDENTIALS_ID>']]])
            }
        }
        stage('Build') {
            steps {
                sh 'echo "build failed" >> log.txt'
                sh 'mkdir .hidden_logs'
                sh 'echo "build failed" | tee -a .hidden_logs/build.log'
                sh 'echo "build failed"'
            }
        }
    }
}

