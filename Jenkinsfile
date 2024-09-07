pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'build'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test'
          }
        }

        stage('API_Test') {
          steps {
            echo 'Running Api test'
          }
        }

      }
    }

  }
}