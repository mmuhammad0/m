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
            echo 'testtettt'
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

    stage('Notify') {
      steps {
        echo 'done'
      }
    }

  }
}