pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'i want to plan my app '
      }
    }

    stage('code') {
      steps {
        echo 'dev'
      }
    }

    stage('build') {
      steps {
        echo 'build app'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test'
          }
        }

        stage('deploy') {
          steps {
            echo 'deploy'
          }
        }

      }
    }

  }
}