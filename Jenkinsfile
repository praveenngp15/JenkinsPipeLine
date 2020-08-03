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
            echo 'deplymentTesting  '
            echo 'Get the driver path${chromeDriverPath}'
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
  environment {
    chromeDriverPath = 'C:\\driver\\web'
  }
}