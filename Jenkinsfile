
pipeline {
  agent none
  stages {
  
    stage('Install Dependencies') {
      steps {
         sh 'npm install'
         }
      }
      
    stage('Test') {
      steps {
         sh 'echo "testing application..."'
         }
      }
      
    stage('build') {
      steps {
         sh 'npm run build'
         }
       }
       
    stage('Deploy application') {
      steps {
         sh 'echo "deploying application..."'
         }
       }
       
     }
    }

