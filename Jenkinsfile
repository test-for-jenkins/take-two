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
        sh 'npm config set cache /tmp'
        sh 'EXPORT HOME=/tmp; npm --prefix install'
        /* sh './node_modules/.bin/jest' */
      }
    }
  }
}
