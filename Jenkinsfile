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
        sh '''if [ -d "javascript" ]; then
  cd javascript
else
  echo "Directory \'javascript\' does not exist."
  exit 1
fi
'''
      }
    }

  }
}