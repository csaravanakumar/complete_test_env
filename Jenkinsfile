pipeline {
   environment {
           }
  agent {label 'EC2StaticJenkinsSlaveFinal'}
  stages {

    stage('Build') {
      steps {
        test()
        }
      }
    

    stage('Unit Test') {
      steps {
        script {
           echo "Unit Testing..."
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
