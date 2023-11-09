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
}