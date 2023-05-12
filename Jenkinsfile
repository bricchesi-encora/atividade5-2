pipeline {
    agent {
        docker {
            image 'openjdk:11'
            args '-v /var/run/docker.sock:/var/run/docker.sock'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'javac OlaUnicamp.java'
            }
        }
        stage('Run') {
            steps {
                sh 'java OlaUnicamp'
            }
        }
    }
}
