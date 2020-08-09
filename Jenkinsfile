pipeline {
   agent {label 'EC2StaticJenkinsSlaveFinal'}
  stages {

    stage('Build') {
      steps {
        script {
           echo "Current build version :: $BUILDVERSION"
           echo "'date +%s'"
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
