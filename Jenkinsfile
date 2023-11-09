pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Building the .NET Core Application'
          }
        }

        stage('Test') {
          steps {
            echo 'Testing the Application'
            echo '"Get the DriverPath $[ChromeDriverPath]"'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy the app in IIS server'
      }
    }

  }
  environment {
    ChromeDriverPath = '/Users/WATSAKAN/Documents'
  }
}