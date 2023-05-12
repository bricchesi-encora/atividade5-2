pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'docker build -t meu-projeto .'
            }
        }
        
        stage('Run') {
            steps {
                sh 'docker run --rm meu-projeto'
            }
        }
    }
}
