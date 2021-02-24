pipeline {
  agent { label 'master' }
  stages {
    stage('DoCheckout') {
      steps {
        script {
          if(isUnix()) {
            sh script: """
            ls
            pwd
            """
          }  else {
             powershell script: """
               ls
               ls env:
             """
          }
          
        }
              }
    }
  }
  
}
