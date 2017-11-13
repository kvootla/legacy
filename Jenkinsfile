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
            sleep 20
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
            sleep 30
          }
        }
        stage('Deploy test') {
          steps {
            echo 'Deploy code begin to testing '
          }
        }
        stage('Trigger build') {
          steps {
            sleep 30
          }
        }
        stage('Trigger integrate testing') {
          steps {
            echo 'Integrating testing has completed successfully '
          }
        }
        stage('Trigger Auto Testing') {
          steps {
            sh '''date
 echo "Auto testing completed successfully"'''
            sleep 30
          }
        }
        stage('Deploy Code') {
          steps {
            sleep 25
          }
        }
      }
    }
    stage('Test Pipeline') {
      steps {
        sleep 30
      }
    }
  }
}