pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'echo build'
          }
        }

        stage('build2') {
          steps {
            sh 'echo build2'
          }
        }

      }
    }

    stage('Test') {
      steps {
        sh 'echo test'
      }
    }

  }
}