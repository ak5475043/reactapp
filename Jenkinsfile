
pipeline {
  agent { node { label 'slave-build-node' } }
  options {
        timeout(time: 1, unit: 'SECONDS')
    }
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
         sh 'sudo cp -r * /var/www/react'
         }
       }
       
     }
    }

