pipeline {
  agent { label '1' } 
  
  triggers { pollSCM '* * * * *' }
  
  tools { nodejs "nodejs" }

  options { timestamps () }
 
  
  stages {    
    stage('Cloning Git') {
      steps { sh  'npm i' }
    }        
  }

}
