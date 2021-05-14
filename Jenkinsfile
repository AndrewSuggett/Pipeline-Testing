pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building'
      }
    }

    stage('Testing') {
      parallel {
        stage('Testing') {
          steps {
            bat 'conda info'
            bat 'conda activate test_reporting'
            bat 'py PipelineTesting.py'
          }
        }

        stage('Input Testing') {
          steps {
            bat 'echo test'
          }
        }

      }
    }

  }
}