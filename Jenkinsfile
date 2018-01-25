#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: '',
    projectUrlStr: 'https://github.com/HelloWorld.git/'],
    pipelineTriggers([githubPush()])])
pipeline{
  agent any
    stages{
      stage('git'){
          steps{
          sh 'git --version'
          sh 'pwd'
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
      stage('Triggering Artifactory Job'){
          steps{
          build 'y0'
          }
      }
     }
  }

