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
                PATH = %SystemRoot%\system32:%PATH%
            bat "mvn clean package"
            }    
        }
    }
 }

