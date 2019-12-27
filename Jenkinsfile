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
      parallel {
        stage('STAGE2') {
          steps {
            echo 'MESSAGE HERE'
          }
        }

        stage('error') {
          steps {
            dir(path: '/var/lib')
          }
        }

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