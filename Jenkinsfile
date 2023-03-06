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
        stage('sonar quality check'){
            steps{
                script{
                withSonarQubeEnv(credentialsId: 'sonar_qube') {
                   sh "mvn clean install sonar:sonar"
                 }
               }
            }
        }
        
        
       
        }

    }
    
