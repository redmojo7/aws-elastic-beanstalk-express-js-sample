pipeline {
  agent {
    docker { 
	label ‘docker-node’
	image 'node:16-alpine' 
	args '-p 3000:3000'
    }
  }
  stages {
    stage('Test') {
      steps {
        sh 'node --version'
      }
    }
    stage('Build') {
      steps {
        sh 'node install -save'
      }
    }
  }
}