pipeline{
    agent any
    
    environment {
    PATH = "C:\\WINDOWS\\SYSTEM32"
    }
        stages{
         stage("git checkout"){
             steps{
               git credentialsId: 'git-hub', url: 'https://github.com/vinodtyagi/webrun.git'
            }
        }
        stage("maven build"){
            steps{
                bat "mvn clean package"
            }    
        }
    }
 }

