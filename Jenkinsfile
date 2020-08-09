pipeline {
  agent {label 'EC2StaticJenkinsSlaveFinal'}
  stages {

    stage('Init') {
      steps {
        script {
          build.setBuildDescription(
            title: "${env.BUILD_NUMBER} My build title.",
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
