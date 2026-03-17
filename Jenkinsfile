pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/ewei03/maven-samples-A6', branch: 'master')
      }
    }

    stage('run') {
      steps {
        bat 'mvn clean'
        bat 'mvn test'
        bat 'mvn verify'
      }
    }

  }
  tools {
    maven 'mvn'
    jdk 'jdk'
  }
}