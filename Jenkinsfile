pipeline {
   environment {
        def BUILDVERSION = env.BUILD_NUMBER
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
           echo "Unit Testing...${BUILDVERSION}"
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
