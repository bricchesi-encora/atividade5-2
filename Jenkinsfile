pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'docker run --rm -v $PWD:/app -w /app maven:3-openjdk-11 mvn compile'
                }
            }
        }
        stage('Run') {
            steps {
                script {
                    sh 'docker run --rm -v $PWD:/app -w /app maven:3-openjdk-11 java -cp target/classes OlaUnicamp'
                }
            }
        }
    }
}
