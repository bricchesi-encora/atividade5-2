pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout do repositório do GitHub
                git 'https://github.com/bricchesi-encora/atividade5-2.git'
            }
        }

        stage('Build') {
            steps {
                // Compilação do código
                sh 'javac OlaUnicamp.java'
            }
        }

        stage('Test') {
            steps {
                // Execução do teste (opcional)
                sh 'echo "Não há testes neste exemplo"'
            }
        }

        stage('Run') {
            steps {
                // Execução do programa
                sh 'java OlaUnicamp'
            }
        }
    }
}
