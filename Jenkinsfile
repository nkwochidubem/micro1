pipeline {
  agent {label 'master' }
  stages {
    stage('Hello') {
      steps {
        echo "hello from micro1 Jenkinsfile"
     }
    }
<<<<<<< HEAD
    stage('test') {
      steps {
        sh '''
        cat *
        '''
      }
    }
=======
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

>>>>>>> 3d5e5310b54c962ce27ff959980ef2ea39910238
  }
}
