pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'HI... Build stage'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            bat 'dir'
            echo 'test'
          }
        }

        stage('test qt') {
          steps {
            sleep 10
          }
        }

      }
    }

  }
}