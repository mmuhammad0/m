pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'nanna'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'test'
          }
        }

        stage('Test1') {
          steps {
            echo 'tee'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'deploy'
      }
    }

  }
}