pipeline {
  agent any
  stages {
    stage('Build Pipeline') {
      parallel {
        stage('Build Pipeline') {
          steps {
            sleep 10
          }
        }
        stage('Code build') {
          steps {
            sh '''date 
echo "Code being simulate for flawless attributes"'''
          }
        }
        stage('Code test') {
          steps {
            echo 'Build being to trigger the code test'
          }
        }
        stage('Code deploy') {
          steps {
            sleep 20
          }
        }
      }
    }
    stage('Deploy Pipeline') {
      parallel {
        stage('Deploy Pipeline') {
          steps {
            sleep 15
          }
        }
        stage('Deploy build') {
          steps {
            sh '''date 
echo "Deploy code triggered to build"'''
          }
        }
      }
    }
  }
}