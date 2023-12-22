pipeline {
  agent none
  stages {
    stage('Buld') {
      steps {
        echo 'This is new build project'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            sh '''mkdir mahi
cd mahi
mkdir mahen.html
ls
pwd
date
cal 2023
git clone https://github.com/ermahen07/jenkins-demo.git
pwd'''
          }
        }

        stage('dploy') {
          steps {
            sleep(time: 10, unit: 'MINUTES')
          }
        }

      }
    }

    stage('prod') {
      steps {
        echo 'this is final production'
      }
    }

  }
  environment {
    Mahender = 'kumar'
  }
}