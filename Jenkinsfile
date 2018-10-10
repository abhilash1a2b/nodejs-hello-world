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
  }
}