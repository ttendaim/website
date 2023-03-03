pipeline {
  agent any
  stages {
    stage('Checkout code') {
      steps {
        git(url: 'https://github.com/ttendaim/curriculum-app', branch: 'dev')
      }
    }

    stage('logs') {
      steps {
        sh 'ls -la'
      }
    }

  }
}