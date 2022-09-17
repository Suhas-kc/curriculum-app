pipeline {
  agent any
  stages {
    stage('Code Checkout') {
      steps {
        git(url: 'https://github.com/Suhas-kc/curriculum-app', branch: 'dev')
      }
    }

    stage('List directory') {
      steps {
        sh 'ls -la'
      }
    }

  }
}