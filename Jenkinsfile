pipeline{
    agent any

    

            tools { 
      maven 'M2_HOME'}

    stages{
         stage('checkout'){
             steps{
                git 'https://github.com/rajdeepsingh642/java-maven-hello.git'
             }
         }
                
         stage('build'){
            steps{
                script{
                 

                    sh 'mvn package'
                }
                }
        }
    }
}