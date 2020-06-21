pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/xbases/tls-cert-expire.git', branch: 'master')
      }
    }

    stage('Build') {
      steps {
        sh 'go run build tls-cert-expire.go'
      }
    }

  }
}