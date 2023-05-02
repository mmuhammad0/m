pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'nannna'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'testtet'
          }
        }

        stage('Test1') {
          steps {
            echo 'tete'
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