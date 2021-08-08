pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Hello'
          }
        }

        stage('Test') {
          steps {
            echo 'Testing'
            echo '"Best is ${player}"'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployed'
      }
    }

  }
  environment {
    player = 'Messi'
  }
}