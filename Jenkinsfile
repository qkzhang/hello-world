pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building..'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing..'
          }
        }

        stage('TestUnit') {
          steps {
            sh 'echo "TestUnit"'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying....'
      }
    }

  }
}