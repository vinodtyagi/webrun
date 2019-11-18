pipeline{
    agent any
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

