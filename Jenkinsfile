pipeline {
  agent {
    docker { dockerfile true }
  }
  stages {
    stage('Test') {
      steps {
        sh 'node --version'
      }
    }
    stage('Build') {
      steps {
        sh 'npm install --save'
      }
    }
  }
}
