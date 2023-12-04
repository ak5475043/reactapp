//
pipeline {
  //agent { node { label 'slave-build-node' } }
  agent any
  stages {
  
    stage('Install Dependencies') {
      steps {
         //sh 'npm install'
         //sh 'sudo cp -r * /home/webexpert/jenkins_test'
         sh 'yarn'
         }
      }
      
    stage('Test') {
      steps {
         sh 'echo "testing application..."'
         }
      }
      
    stage('build') {
      steps {
         //sh 'npm run build'
         sh 'echo "building application..."'
         }
       }
       
    stage('Deploy application') {
      steps {
         //sh 'sudo cp -r * /var/www/react'
         sh 'echo "deploying application..."'
         }
       }
       
     }
    }

