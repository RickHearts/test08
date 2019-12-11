pipeline {
  agent any
  stages {
    stage('Chrome') {
      steps {
        echo 'Chrome Test'
      }
    }

    stage('Firefox') {
      parallel {
        stage('Firefox') {
          steps {
            echo 'Firefox Test'
          }
        }

        stage('Mozilla') {
          agent {
            node {
              label 'ubuntu_slave1'
            }

          }
          steps {
            echo 'Mozilla Message'
          }
        }

      }
    }

  }
}