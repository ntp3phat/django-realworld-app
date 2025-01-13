pipeline {
  agent any
  stages {
    stage('checkout Code') {
      steps {
        git(url: 'https://github.com/ntp3phat/django-realworld-app.git', branch: 'master')
      }
    }

    stage('build image') {
      steps {
        sh 'sh \'docker build -t realworld-python:1.0 .\''
      }
    }

  }
}