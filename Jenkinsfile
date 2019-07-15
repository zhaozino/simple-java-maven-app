pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        bat(encoding: 'utf-8', script: 'bat \'mvn -B -DskipTests clean package\' ', label: 'BuildLabel')
        sh 'npm install'
      }
    }
  }
}