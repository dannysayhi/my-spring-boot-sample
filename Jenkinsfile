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
        sh 'mvn test'
        archiveArtifacts 'target/surefire-reports/*.xml'
      }
    }
  }
}