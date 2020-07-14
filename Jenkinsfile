pipeline {
  agent node { label '1' } 
  
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
