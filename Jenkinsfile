pipeline {
  agent {
    docker {
      image 'node:latest'
    }
  }
  stages {
    stage('Test') {
      steps {
        sh 'echo $USER'
        sh 'node --version'
        /* sh 'npm install' */
        /* sh './node_modules/.bin/jest' */
      }
    }
  }
}
