pipeline {
  agent any
  tools {
    maven 'M3'
  }
  stages {
    stage('Build') {
      steps {
        echo 'sample project'
        sh 'mvn clean'
      }
    }
  }
}
