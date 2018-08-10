pipeline {
  agent any
  stages {
    stage('HelloWord') {
      parallel {
        stage('HelloWord') {
          steps {
            echo 'Helloword'
          }
        }
        stage('RemotePowerShell') {
          steps {
            powershell(script: 'CD D:', returnStdout: true, returnStatus: true)
          }
        }
      }
    }
  }
}