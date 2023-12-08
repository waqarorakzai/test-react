pipeline {
  agent any
 
  tools {nodejs "NodeJs21"}
 
  stages {
    stage('Test NPM') {
      steps {
        sh 'npm config ls'
      }
    }

    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }
     
    stage('Test') {
      steps {
         sh 'npm start'
      }
    }     
  }
}
