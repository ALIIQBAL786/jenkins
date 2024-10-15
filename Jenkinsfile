pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing'
          }
        }

        stage('Test sar') {
          steps {
            echo 'Test sar'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy to Prod'
      }
    }

  }
}