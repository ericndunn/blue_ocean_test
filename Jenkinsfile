pipeline {
  agent any
  stages {
    stage('STAGE1') {
      parallel {
        stage('STAGE1') {
          steps {
            sh 'echo "Hello"'
          }
        }

        stage('error') {
          steps {
            sh 'echo "World"'
          }
        }

      }
    }

    stage('STAGE2') {
      steps {
        echo 'MESSAGE HERE'
      }
    }

    stage('STAGE3') {
      steps {
        sh 'echo "Hello World!"'
      }
    }

  }
  environment {
    NAME = 'VALUE'
  }
}