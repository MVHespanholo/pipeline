pipeline {
    agent any 

    stages {
        stage('Build') {
            steps {
                echo "construindo....."
                sh '''
                cd comandos
                ls
                cat requisito
                '''
                echo "terminado"
            }
        }
        stage('Test') {
            steps {
                echo "testando"
                sh '''
                cd comandos
                ls
                python3 olamundo.py   
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
