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
            build(propagate: true, wait: true, quietPeriod: 1, job: 'Build')
          }
        }
        stage('Code test') {
          steps {
            echo 'Build being to trigger the code test'
          }
        }
      }
    }
  }
}