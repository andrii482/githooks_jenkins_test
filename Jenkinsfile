pipeline {
  agent any
  
  triggers { pollSCM '* * * * *' }
  
  tools {nodejs "nodejs"}

  options { timestamps () 
            ansiColor('xterm') 
          }
 
  
  stages {    
    stage('Cloning Git') {
      steps { sh  'npm i' }
    }        
  }
  post { 
    always { cleanWs()}
  }
}
