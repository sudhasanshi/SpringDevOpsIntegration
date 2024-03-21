pipeline {
  tools {
  maven 'maven'
  }
  agent any
  stages {
    stage('checkout') {
      steps {
        sh 'rm -rf  hello-world-war'
        sh 'git clone https://github.com/sudhasanshi/hello-world-war.git'
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
