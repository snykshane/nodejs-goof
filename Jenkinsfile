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
        snykSecurity(additionalArguments: '-d', organisation: '11347754-fadd-415d-826f-80bc248f5348', projectName: 'snykshane/nodejs-goof', snykTokenId: '9110fd08-4ef4-4898-a216-3b3a65bc3cd9')
      }
    }

  }
}