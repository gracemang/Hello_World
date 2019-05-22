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
        stage('Step') {
          steps {
            sh '''max = 5
for((i=2; i <= $max; ++i))

do 

echo "$i"

done'''
          }
        }
      }
    }
  }
}