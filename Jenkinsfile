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
            echo "Best is ${player} "
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        input 'Want to deploy?'
        echo 'Deployed'
      }
    }

  }
  environment {
    player = 'Henry'
  }
}