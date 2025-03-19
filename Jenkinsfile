pipeline {
  agent any
  tools {
    maven 'maven3.9.9'
    jdk 'jdk1.8'
  }
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/hansraj09/maven-samples.git', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn verify'
      }
    }

  }
}
