pipeline {
  agent {
    docker {
      args '-p 3000:3000'
      image 'node:8-alpine'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'mpn install'
      }
    }
    stage('Test') {
      steps {
        sh 'npm test'
      }
    }
  }
}