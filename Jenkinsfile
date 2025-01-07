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

    stage('Front end Test') {
      steps {
        sh '''if [ -d "javascript-front" ]; then
  cd javascript-front
else
  echo "Directory \'javascript-front\' does not exist."
  exit 1
fi
'''
      }
    }

  }
}