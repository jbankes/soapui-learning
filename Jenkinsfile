pipeline {
  agent none

  stages {
    stage('Run Soap UI') {
      agent {
        docker { image 'ddavison/soapui:5.4.0'}
      }
      steps {
        sh 'curl --form "project=@soapui-project.xml" http://localhost:3000'
      }
    }
  }
}