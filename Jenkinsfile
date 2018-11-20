pipeline {
     
	currentBuild.result = "SUCCESS"
	
	agent any
	
	 try {
	
	
     stages{
         stage('Init'){
             steps{
                echo "Testing...."
             }
          }
 
         stage('Build'){
             steps{
                echo "Building...."
             }
          }

	 stage('Deploy'){
             steps{
                echo "Code Deployed...."
             }
          }
       
	   stage('Cleanup'){
	   	         steps{
                echo "Build Successful...."
             }
	      }
    	
      }	
	 } 
	 catch (err) {
       currentBuild.result = "FAILURE"
       throw err	 
	  	  
	}
	
}
	
	
     
