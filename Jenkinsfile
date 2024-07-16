pipeline {
  agent none
  stages {
    stage('frontend') {
      agent {
        docker ( image 'maven:3.9.8-eclipse-temurin-11' )
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
