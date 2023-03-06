pipeline{
    agent any

    

    stages{
         stage('checkout'){
             steps{
                
         stage('build'){
            steps{
                script{
                    sh 'mvn compile'
                    sh 'mvn package'
                }
                }
        }
    }
}