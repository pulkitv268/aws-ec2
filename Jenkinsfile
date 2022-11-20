#!groovy

pipeline {
	agent none
  stages {
    stage('Docker Build') {
    	agent any
      steps {
      	sh 'docker build . -t todo .'
	sh 'docker run -p 8000:8000 -d todo'
      }
    }
  }
}
