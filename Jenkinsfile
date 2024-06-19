pipeline {
    agent any 

    stages {
        stage('Build') {
            steps {
                echo "construindo....."
                bat '''
                cd comandos
                dir
                type requisito
                '''
                echo "terminado"
            }
        }
        stage('Test') {
            steps {
                echo "testando"
                bat '''
                cd comandos
                dir
                python olamundo.py   
                '''
                echo "teste completo"
            }
        }
        stage('Deliver') {
            steps {
                echo "entregando"
                echo "entrega completa"
            }
        }
    }
}
