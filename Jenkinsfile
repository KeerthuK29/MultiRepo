pipeline{
    agent any
    stages{
        stage('Checkout') {
            steps {
                
                git branch: 'main', url: 'https://github.com/KeerthuK29/MultiRepo.git/'
            }
        }
        stage('Build'){
            steps{
                script {
                  bat 'javac Main.java'
                   
                }
            }
        }
        stage('Run'){
            steps{
                script{
                    bat 'java Main'
                   
                }
            }
        }
    }
}
