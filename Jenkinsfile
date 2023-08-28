pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'I want to build'
      }
    }

    stage('test') {
      steps {
        echo 'I want to test'
      }
    }

    stage('stage') {
      parallel {
        stage('stage') {
          steps {
            echo 'I want to stage'
          }
        }

        stage('deploy') {
          steps {
            echo 'I want to deploy'
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