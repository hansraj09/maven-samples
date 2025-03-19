pipeline {
  agent any
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