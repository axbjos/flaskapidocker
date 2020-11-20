//pipeline
pipeline {
  agent { docker { image 'python:latest' }}
  stages {
    stage('build') {
      steps {
        sh 'pip install --no-cache-dir -r requirements.txt'
      }
    }
    stage('test') {
      steps {
        sh 'python test.py'
      }   
    }
  }
}
