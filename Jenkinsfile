pipeline{
  agent any
  stages{
    stage('checkout') {
      steps {
        git 'https://github.com/GODGALAXY289/Devops-Lab.git'
      }
    }
    stage('Publish') {
      steps {
        publishHTML([
          allowMissing:true,
          alwaysLinkToLastBuild:false,
          keepAll:false,

          reportDir:'.',
          reportFiles:'Temporary.html',
          reportName:'My html pipe page'
        ])
      }
    }
  }
}
