pipeline {
  agent any
  
  triggers {
 /*   - github-pull-request:
        cron: '* * * * *'
        github-hooks: true
        permit-all: true
        auto-close-on-fail: false
        started-status: "started"
        status-add-test-results: "test result with status message"
        success-status: "success message"
        failure-status: "failure message"
        error-status: "error message"
        success-comment: "success comment"
        failure-comment: "failure comment"
        error-comment: "error-comment"
        cancel-builds-on-update: true */ }
  
  tools {nodejs "nodejs"}

  options { timestamps () 
            ansiColor('xterm') 
          }
 
  
  stages {    
    stage('Cloning Git') {
      steps {
        sh  'npm i' 
      }
    }        
  }
  post { 
    always { 
      cleanWs()
    }
  }
}
