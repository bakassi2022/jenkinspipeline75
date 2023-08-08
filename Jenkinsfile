pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'I want to build'
      }
    }

    stage('Test') {
      steps {
        echo 'I want to test'
      }
    }

    stage('Stage') {
      parallel {
        stage('Stage') {
          steps {
            echo 'I want to stage'
          }
        }

        stage('deploy') {
          steps {
            echo 'want to deploy'
          }
        }

        stage('operate') {
          steps {
            echo 'I want to operate'
          }
        }

      }
    }

  }
}