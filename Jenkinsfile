pipeline {
  agent any
  stages {
    stage('Code Checkout') {
      steps {
        git(url: 'https://github.com/Suhas-kc/curriculum-app', branch: 'dev')
      }
    }

    stage('List directory') {
      parallel {
        stage('List directory') {
          steps {
            sh 'ls -la'
          }
        }

        stage('Frontend unit test') {
          steps {
            sh 'cd curriculum-front && npm i && npm run test:unit'
          }
        }

      }
    }

  }
}