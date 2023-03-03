pipeline {
  agent any
  stages {
    stage('Checkout code') {
      steps {
        git(url: 'https://github.com/ttendaim/website', branch: 'main')
      }
    }

    stage('Shell script') {
      steps {
        sh 'ls -la'
      }
    }

  }
}