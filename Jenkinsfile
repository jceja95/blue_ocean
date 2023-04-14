pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo '"testing"'
          }
        }

        stage('Parallel') {
          steps {
            echo 'parallel running'
          }
        }

      }
    }

    stage('') {
      steps {
        echo 'building'
      }
    }

    stage('Clean up') {
      steps {
        echo 'cleaning up'
      }
    }

  }
}