pipeline {
  agent {label 'master' }
  stages {
    stage('Hello') {
      steps {
        echo "hello from micro1 Jenkinsfile"
     }
    }
    stage('test') {
      steps {
        sh '''
        cat *
        '''
      }
    }
  }
}
