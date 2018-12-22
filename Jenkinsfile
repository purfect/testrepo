pipeline {
  agent any
  parameters {
    booleanParam(name: 'do_deployment', defaultValue: false, description: 'Aktivieren um Deployment durchzuführen')
  }
  stages {
    stage('stage 1') {
      when { expression { return params.do_deployment } }
      steps {
        sh "/bin/bash testscript.sh && ls"
      }
    }
  }
}

