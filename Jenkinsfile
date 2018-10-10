pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'npm i'
      }
    }
    stage('run') {
      steps {
        sh 'node server.js'
      }
    }
    stage('expose') {
      steps {
        sh 'docker run --net host -ti jpetazzo/ngrok http localhost:1337'
      }
    }
  }
}