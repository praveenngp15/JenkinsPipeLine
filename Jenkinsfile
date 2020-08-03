pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Building Java Application'
          }
        }

        stage('Test') {
          steps {
            echo 'deplymentTesting the '
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying the application'
      }
    }

  }
}