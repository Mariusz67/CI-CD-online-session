pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build phase'
      }
    }

    stage('Build2') {
      steps {
        script {
          def customImage = docker.build("${registry}:${env.BUILD_ID}")
        }

      }
    }

  }
}