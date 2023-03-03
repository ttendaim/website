pipeline {
  agent any
  stages {
    stage('Checkout code') {
      steps {
        git(url: 'https://github.com/ttendaim/curriculum-app', branch: 'dev')
      }
    }

    stage('logs') {
      parallel {
        stage('logs') {
          steps {
            sh 'ls -la'
          }
        }

        stage('Front-End') {
          steps {
            sh '''cd curriculum-front && npm ci && npm run test:unit
'''
          }
        }

      }
    }

  }
}