pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building'
      }
    }

    stage('Testing') {
      steps {
        bat(script: 'RunScipt.bat', returnStatus: true)
      }
    }

  }
}