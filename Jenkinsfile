pipeline {
  agent any
  stages {
    stage('stg1') {
      steps {
        sh 'pwd'
      }
    }
    stage('stg2') {
      steps {
        parallel(
          "stg2": {
            sh 'ls'
            
          },
          "par": {
            sh 'ls'
            
          }
        )
      }
    }
    stage('stg3') {
      steps {
        sh 'ls'
      }
    }
  }
  environment {
    k = 'v'
  }
}