pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        bat 'npm install -g @angular/cli && npm install && ng build --prod'
      }
    }
    stage('deploy') {
      steps {
        bat 'firebase deploy'
      }
    }
  }
}
