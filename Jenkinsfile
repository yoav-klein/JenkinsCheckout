pipeline {
 /* options {
   skipDefaultCheckout() 
  }*/
  agent { label 'master' }
  stages {
    stage('DoCheckout') {
      steps {
        checkout scm
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
