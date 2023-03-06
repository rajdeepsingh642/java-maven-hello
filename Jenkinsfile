pipeline{
    agent any

     tools { 
      maven  'mymaven'
     }

    stages{
         stage('checkout'){
             steps{
                git 'https://github.com/rajdeepsingh642/java-maven-hello.git'
             }
         }
                
         stage('build'){
            steps{
                script{
                 

                    sh 'mvn clean package'
                }
                }
        }
    }
}