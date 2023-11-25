pipeline {
  agent any
  stages {
    stage('Chceckout') {
      environment {
        registry = 'mariusz67/mp_devops_test'
      }
      steps {
        script {
          checkout scm
        }

      }
    }

    stage('Build') {
      steps {
        script {
          def customImage = docker.build("${registry}:${env.BUILD_ID}")
        }

      }
    }

  }
}