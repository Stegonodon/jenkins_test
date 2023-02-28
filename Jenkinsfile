pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        dir('/home/azureuser/je2') {
          sh 'npm install'
          sh 'npm run build'
        }
      }
    }
    stage('Test') {
      steps {
        sh 'npm test'
      }
    }
    stage('Deploy') {
      steps {
        sh 'npm run deploy'
      }
    }
  }
}
