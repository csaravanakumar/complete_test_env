pipeline {
   environment {
        def BUILDVERSION = sh(script: "echo `date +%s`", returnStdout: true).trim()
        def formattedDate = aDate.format("EEE, MMMM dd, yyyy, hh:mm a '('zzz')'", TimeZone.getTimeZone(siteConfig.getString("timeZone")))
               }
  agent {label 'EC2StaticJenkinsSlaveFinal'}
  stages {

    stage('Build') {
      steps {
        script {
           echo "Current build version :: ${BUILDVERSION}"
           echo "Current build version :: ${formattedDate}"
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
