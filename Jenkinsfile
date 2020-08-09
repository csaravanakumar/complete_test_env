pipeline {
   environment {
        def BUILDVERSION = sh(script: "echo `date +%s`", returnStdout: true).trim()
    }
  agent {label 'EC2StaticJenkinsSlaveFinal'}
  stages {

    stage('Init') {
      steps {
        script {
          build.setBuildDescription(
            title: "${BUILDVERSION} My build title.",
            description: 'My build description.'
          )
        }
      }
    }

    stage('Build') {
      steps {
        script {
          echo 'Building...'
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
