pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        sh 'g++ new.cpp -o new'
      }
    }
   
    stage('Test') {
      steps {
        sh './new'
      }
    }
   
    stage('Deploy') {
      steps {
        sh ''
      }
    }
  }
 
  post {
    failure {
       
          echo 'Pipeline failed'
        }
    }
   
  }
