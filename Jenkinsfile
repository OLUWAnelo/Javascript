pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/OLUWAnelo/Javascript', branch: 'main')
      }
    }

    stage('Log') {
      steps {
        sh 'ls -la'
      }
    }

    stage('FrontEnd Test') {
      steps {
        sh 'cd javascript && npm i && npm run test:unit '
      }
    }

  }
}