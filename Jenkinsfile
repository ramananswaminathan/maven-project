pipeline {
    	
	agent any
	
     stages{
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
     }		
          
		  post {
   
			success {
				echo "success"
					}
			failure {
				echo "failiure"
				 mail to:"ramanan.swaminathan@gmail.com", subject:"FAILURE: ${currentBuild.fullDisplayName}", body: "Boo, we failed."

					}
				}

  }
		  
		  
		  
		  
		  
		  
	
	   
	
     
