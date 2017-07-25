pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        parallel(
          "stage1": {
            sh 'echo toto'
            
          },
          "": {
            sh 'ls -la'
            
          }
        )
      }
    }
  }
}