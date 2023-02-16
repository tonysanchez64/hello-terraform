pipeline {
    agent any

    stages {
        stage('terraform') {
              withAWS(credentials: 'credenciales-aws', region: 'eu-west-1') {
                        sh 'terraform apply -auto-approve'
              }
            
            }
        }
    }
}
