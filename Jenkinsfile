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
          steps {
            echo 'Mozilla Message'
          }
        }

      }
    }

  }
}