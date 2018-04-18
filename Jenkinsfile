pipeline {
  agent any
  stages {
    stage('checkout project') {
      steps {
        checkout scm
      }
    }
    stage('test/') {
      steps {
        archiveArtifacts 'target/surefire-reports/*.xml'
      }
    }
  }
}