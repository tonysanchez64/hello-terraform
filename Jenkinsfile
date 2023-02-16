pipeline {
    agent any

    stages {
        stage('terraform') {
              steps{
                   withAWS(credentials: 'credenciales-aws', region: 'eu-west-1') {
                        sh 'terraform init'
                        sh 'terraform apply -auto-approve'
                   }
              }
        }
    }
}
