pipeline {
  agent any
  stages {
    stage('Say Hello') {
      steps {
        echo 'Hello World!'
        sh 'java -version '
      }
    }
    stage('Hello World ') {
      steps {
        sh '''pipeline {
  agent {
    label \'jdk10\'
  }
  stages {
    stage(\'Say Hello\') {
      steps {
        echo \'Hello World!\'
        sh \'java -version \'
      }
    }
  }
}'''
        }
      }
    }
  }