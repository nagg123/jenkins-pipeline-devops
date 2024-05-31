pipeline {
  agent any
  stages {
    stage('code') {
      steps {
        echo 'start the code'
      }
    }

    stage('build') {
      steps {
        echo 'build the code'
      }
    }

    stage('test') {
      steps {
        echo 'test the code'
      }
    }

    stage('staging') {
      parallel {
        stage('staging') {
          steps {
            echo 'staging the code'
          }
        }

        stage('production') {
          steps {
            echo 'product the code'
          }
        }

      }
    }

  }
}