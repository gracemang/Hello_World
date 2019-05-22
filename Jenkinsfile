pipeline {
  agent any
  stages {
    stage('Initialize') {
      steps {
        echo 'Starting testing'
      }
    }
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Starting Build'
          }
        }
        stage('') {
          steps {
            sh '''for(int i =0; i < 5; i++){
echo \'Hello World\'
}'''
            }
          }
        }
      }
    }
  }