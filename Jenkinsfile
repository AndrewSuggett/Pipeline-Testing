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
        bat(script: 'RunScript', returnStdout: true)
      }
    }

  }
}