pipeline {
  agent {
    docker {
      image 'node:latest'
      args '-p 3000:3000'
    }
  }
  stages {
    stage('Test') {
      withDockerContainer(args: '-u root') {
        sh 'echo $USER'
        sh 'npm install'
        sh './node_modules/.bin/jest'
      }
    }
  }
}
