pipeline {
  agent {
    docker {
      image 'mhart/alpine-node:8'
    }
  }
  stages {
    stage('Test') {
      steps {
        sh 'echo $USER'
        sh 'node --version'
        sh 'npm install'
        /* sh 'npm config set cache /tmp' */
        /* sh 'EXPORT HOME=/tmp; npm --prefix install' */
        sh './node_modules/.bin/jest'
      }
    }
  }
}
