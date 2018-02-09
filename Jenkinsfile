pipeline {
  agent any
  stages {
    stage('error') {
      environment {
        tesr = 'test'
      }
      parallel {
        stage('error') {
          steps {
            echo 'HELLO'
          }
        }
        stage('test') {
          steps {
            timeout(time: 12) {
              sleep 1
            }
            
            echo 'tesr'
          }
        }
      }
    }
    stage('toto') {
      steps {
        echo 'yyy'
      }
    }
  }
}