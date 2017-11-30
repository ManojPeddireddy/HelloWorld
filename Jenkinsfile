pipeline{
  agent any
    stages{
      stage('git'){
          steps{
          sh 'git --version'
          sh 'pwd'
          sh 'cd gitproj'
          sh 'git remote add origin https://github.com/ManojPeddireddy/HelloWorld.git'
          sh 'git pull origin'
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
