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

  }
}