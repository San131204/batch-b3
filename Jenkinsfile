pipeline {
    agent any

    stages {
        stage('clone') {
            steps {
                git branch: 'main', credentialsId: '3004c062-a307-4fce-b3de-f15626c698da', url: 'https://github.com/San131204/batch-b3.git'
            }
        }
        stage('compile') {
            steps {
                bat 'javac HelloWorld.java'
            }
        }
        stage('run') {
            steps {
                bat 'java HelloWorld'
            }
        }
    }
}

