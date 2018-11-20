node {
    	

	
     try {
         stage('Init'){
             steps{
                echo "Testing...."
             }
          }
 
         stage('Build'){
             steps{
                echo Building...."
             }
          }

	 stage('Deploy'){
             steps{
                echo "Code Deployed...."
             }
			 
		}
    	
    } catch (err) {

        currentBuild.result = 'FAILED'

        throw err

    }      
		  

  }
		  
		  
		  
		  
		  
		  
	
	   
	
     
