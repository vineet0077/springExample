pipeline {
  agent {
    docker {
      image 'maven:3.5.4-jdk-10'
    }

  }
  stages {
    stage('Build') {
      steps {
        bat 'mvn clean'
      }
    }
    stage('Test') {
      steps {
        bat 'mvn test'
      }
    }
    stage('Deploy') {
      steps {
        bat 'mvn package'
      }
    }
  }
}