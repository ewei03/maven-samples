pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/ewei03/maven-samples', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn verify'
      }
    }

  }
}