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
        bat 'conda info'
        bat 'conda activate test_reporting'
        bat 'py PipelineTesting.py'
      }
    }

  }
}