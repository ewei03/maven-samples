pipeline {
  agent any

  tools { 
    maven 'mvn'
    jdk 'jdk'
  }

  stages {
    stage('check out') {
      steps {
        git url: 'https://github.com/ewei03/maven-samples', branch: 'master'
      }
    }

    stage('run') {
      steps {
        bat 'mvn verify'
      }
    }
  }
}
