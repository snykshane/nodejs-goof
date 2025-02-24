pipeline {
  agent any
  stages {
    stage('Code Checkout') {
      steps {
        git 'https://github.com/snykshane/nodejs-goof'
      }
    }

    stage('snykcheck') {
      steps {
        snykSecurity(additionalArguments: '-d')
      }
    }

  }
}