pipeline {
  agent any
  stages {
    stage('STAGE1') {
      parallel {
        stage('STAGE1') {
          steps {
            cleanWs()
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

    stage('') {
      steps {
        bat(script: 'set', label: 'windows', returnStdout: true, returnStatus: true)
      }
    }

  }
  environment {
    NAME = 'VALUE'
  }
}