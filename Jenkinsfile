pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'mvn  clean'
      }
    }
    stage('Compile') {
      steps {
        bat 'mvn  install'
      }
    }
    stage('Test') {
      steps {
        echo 'Test Completed!'
      }
    }
    stage('Deploy') {
      steps {
        bat 'copy target\\*.jar F:\\mule_server\\mule-enterprise-standalone-4.2.1\\apps'
      }
    }
  }
}