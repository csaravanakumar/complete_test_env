pipeline {
   environment {
        def BUILDVERSION = sh(script: "echo `date +%s`", returnStdout: true).trim()
    }
  agent {label 'EC2StaticJenkinsSlaveFinal'}
  stages {

    stage('Build') {
      steps {
        script {
           echo 'Building...${BUILDVERSION}'
        }
      }
    }

    stage('Unit Test') {
      steps {
        script {
          echo 'Unit Testing...'
        }
      }
    }

    stage('Deploy') {
      steps {
        script {
          echo 'Deploying...'
        }
      }
    }

  }
}
