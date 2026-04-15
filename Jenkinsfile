pipeline {
    agent any

    tools {
        nodejs 'nodejs'
    }

    stages {
        stage('Instalação das dependências') {
            steps {
                echo 'Instalando os pacotes node...'
                bat 'npm install'
            }     
       }

       stage('Execução dos testes') {
            steps {
                echo 'Executando os testes...'
                bat 'npm test'
            }     
       }
    }

    post {
        success {
            echo 'Build e testes executados com sucesso!'
        }
        failure {
            echo 'Build ou testes falharam. Verifique os logs para mais detalhes.'
        }
    }



}