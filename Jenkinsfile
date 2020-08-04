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
            echo 'deplymentTesting'
            echo "Get the driver path${chromeDriverPath}"
          }
        }

        stage('TestLog') {
          steps {
            writeFile(file: 'LogTestFile.txt', text: 'This is an automated test file')
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        input(message: 'Do you want to deploy', id: 'OK')
        echo 'Deploying the application into server'
      }
    }

  }
  environment {
    chromeDriverPath = 'C:\\driver\\web'
  }
}