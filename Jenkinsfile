pipeline {
  agent none
  stages {
    stage('frontend') {
      agent {
        docker ( image 'maven:latest' )
      }
      steps {
        sh 'mvn --version'
      }
    }
    
    stage('backend') {
      agent {
        docker ( image 'node:16-alpine' )
      }
      steps {
        sh 'node --version'
      }
    }
  }
}
