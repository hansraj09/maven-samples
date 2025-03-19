pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/hansraj09/maven-samples.git', branch: 'master')
      }
    }

    stage('test') {
      steps {
        sh 'mvn test'
      }
    }

    stage('verify') {
      steps {
        sh 'mvn verify'
      }
    }

    stage('clean') {
      steps {
        sh 'mvn clean'
      }
    }

  }
  tools {
    maven 'maven3.9.9'
    jdk 'jdk1.8'
  }
}