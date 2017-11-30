pipeline{
  agent any
    stages{
      stage('git'){
          steps{
          sh 'git --version'
          sh 'pwd'
          sh 'cd gitproj'
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
