pipeline{
  agent any
  stages{
    stage('checkout') {
      step {
        git 'https://github.com/GODGALAXY289/Devops-Lab.git'
      }
    }
    stage('Publish') {
      steps {
        publishHTML([
          allowmissing:true,
          alwaysLinktoLastBuild:false,
          KeepAll:false,

          reportDir:'.',
          reportFiles:'Temporary.html'
          reportName:'My html pipe page'
        ])
      }
    }
  }
}
