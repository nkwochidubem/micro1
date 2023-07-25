pipeline {
  agent {label 'master' }
  stages {
    stage('Hello') {
      steps {
        sh '''
          echo "hello from micro1 Jenkinsfile"
          cat *
        '''
     }
    }
    stage('For fix branch'){
     when {
         branch "fix-*"
     } 
     steps {
       sh '''
          cat README.md
       '''
     }
   }
   stage('For the PR'){
     when {
         branch "PR-*"
     }
     steps {
      echo 'this only runs for the PRs'
     }
   }

  }
}
