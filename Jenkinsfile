pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/lion2240/java-hello-world.git', branch: 'master')
        sh 'javac HelloWorld.java'
      }
    }
    stage('Deploy') {
      steps {
        sh 'java HelloWorld'
      }
    }
  }
}