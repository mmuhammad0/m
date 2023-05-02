pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'nafnna'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'testttt'
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
        input(message: 'deploy?', ok: 'deploy')
        echo 'deploy'
      }
    }

   

  }
}