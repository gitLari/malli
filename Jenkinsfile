pipeline {
  agent {
    docker {
      image 'node:8-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Phase 1: new phase (Build)') {
      steps {
        sh 'npm install'
      }
    }
    stage('Phase 2: New phase (test)') {
      steps {
        sh 'npm test'
      }
    }
  }
}