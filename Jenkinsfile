pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            git(url: 'https://github.com/kanthibushan', branch: 'Test1')
          }
        }
        stage('Test') {
          steps {
            echo 'Test'
          }
        }
      }
    }
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test'
          }
        }
        stage('') {
          steps {
            echo 'Test'
          }
        }
      }
    }
  }
}