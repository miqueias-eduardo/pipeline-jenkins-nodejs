Pipeline{
    agent any
    stages{
        stage('Instalar dependências'){
            steps{
                bat 'npm install'
            }
        }

        stage('Build'){
            steps{
                bat 'npm run build'
            }
        }

        stage('Testes'){
            steps{
                bat 'npm test'
            }
        }
        
    }
    
    post {
            success{
                echo "Pipeline executada com sucesso"
            }

            failure {
            echo "Pipeline falhou"
        }
        }

}