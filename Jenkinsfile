pipeline {
  agent {
    docker {
      image 'node:latest'
      args '-p 3000:3000'
    }
  }
  stages {
    stage('Test') {
      steps {
        sh './node_modules/.bin/jest'
      }
    }
  }
}
