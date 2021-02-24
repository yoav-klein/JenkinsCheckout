pipeline {
  agent { label 'linux' }
  stages {
    stage('DoCheckout') {
      steps {
        sh script: """
          ls
          pwd
        """
      }
    }
  }
  
}
