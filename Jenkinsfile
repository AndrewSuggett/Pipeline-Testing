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
        bat(script: 'RunScript.bat', returnStatus: true, returnStdout: true)
        bat 'python --version'
      }
    }

  }
}