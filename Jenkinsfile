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
            echo 'Testing'
          }
        }

        stage('Parallel') {
          steps {
            echo 'still testing'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo 'build'
      }
    }

    stage('Clean up') {
      steps {
        echo 'clean up'
      }
    }

  }
}