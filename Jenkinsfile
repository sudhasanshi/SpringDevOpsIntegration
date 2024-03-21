pipeline {
  tools {
  maven 'maven'
  }
  agent any
  stages {
    stage('checkout') {
      steps {
        sh 'rm -rf  SpringDevOpsIntegration'
        sh 'git clone https://github.com/sudhasanshi/SpringDevOpsIntegration.git'
      }
    }
    stage('build') {
      steps {
        sh 'mvn --version'
        sh 'mvn clean install'
      }
    }
  }
}
