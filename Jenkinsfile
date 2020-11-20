//pipeline
pipeline {
  agent { docker { image 'python:latest' }}
  stages {
    stage('build') {
      steps {
        sh 'pip3 install --no-cache-dir -r requirements.txt --user' 
      }
    }
    stage('test') {
      steps {
        sh 'python3 test.py'
      }   
    }
  }
}
