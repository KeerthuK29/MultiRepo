pipeline{
    agent any
    stages{
        stage('Checkout') {
            steps {
                
                git branch: 'dev', url: 'https://github.com/KeerthuK29/MultiRepo.git/'
            }
        }
        stage('Build'){
            steps{
                script {
                    bat 'javac Method.java'
                }
            }
        }
        stage('Run'){
            steps{
                script{
                  
                    bat 'java Method'
                }
            }
        }
    }
}
