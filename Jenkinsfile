pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        catchError() {
          sh 'sudo filebot -script fn:amc --output /media --log-file /tmp/amc_sort_good.log --action move -non-strict /media/Sort --def clean=y --lang fr --def skipExtract=y --def music=y --filter "rating > 5" --conflict auto'
        }
        
      }
    }
  }
}