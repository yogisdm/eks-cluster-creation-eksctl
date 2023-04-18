pipeline {
  
  agent any  
  
  stages {
    stage('checkout') {
      steps {
        checkout scm
  	    }
    	}
    
 
    stage('eks cluster creation') {
      steps {
	   sh 'eksctl create cluster -f cluster-creation.json'
		    timeout(time: 30, unit: 'MINUTES') {
                    
                } 
      }
    }
	

  }
  
  
}