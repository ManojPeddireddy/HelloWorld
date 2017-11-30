pipeline{
  agent any
    stages{
      stage('git'){
          steps{
          sh 'git -version'
          sh 'pwd'
          sh 'mkdir gitproj'
          sh 'cd gitproj'
          sh 'git init'
          sh 'git clone https://github.com/ManojPeddireddy/HelloWorld.git'
          sh 'git pull'
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
