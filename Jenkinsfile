pipeline{
  agent any
    stages{
      stage('git'){
          steps{
          sh 'git --version'
          sh 'pwd'
          sh 'git remote add origin git://github.com/ManojPeddireddy/HelloWorld.git'  
          sh 'git remote -v'
          sh 'git pull origin master'
          sh 'ls'
          }
       }   
       stage('Maven'){
          steps{
          sh 'mvn --version'
          sh 'mvn clean install'
          }
        }
     }
  }
