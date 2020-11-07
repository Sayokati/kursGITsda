pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/Sayokati/kursGITsda', branch: 'master')
      }
    }

    stage('Maven build') {
      steps {
        sh '''echo %cd% 
cd C:\\Testy\\selenium-training-master 
echo %cd% 
mvn build'''
      }
    }

  }
  environment {
    BRANCH = 'master'
  }
}