pipeline{
    agent any
        stages{
         stage("git checkout"){
             steps{
               git credentialsId: 'git-hub', url: 'https://github.com/vinodtyagi/webrun.git'
            }
        }
        stege{
            steps("maven build")
            bat "mvn clean package"
        }
    }
 }

