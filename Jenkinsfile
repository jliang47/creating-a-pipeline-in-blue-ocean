pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo build'
      }
    }

    stage('test') {
      steps {
        sh 'echo test'
        withSonarQubeEnv('sonar_demo') {
          waitForQualityGate true
        }

      }
    }

  }
}