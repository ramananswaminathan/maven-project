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

                echo "Building...."

             }

          }



		stage('Deploy'){

             steps{

                echo "Code Deployed...."

             }

			 

		}

     }		

          
		  post {

           	 always {
            emailext body: 'A Test EMail 33', recipientProviders: [[$class: 'DevelopersRecipientProvider'], [$class: 'RequesterRecipientProvider']], subject: 'Test'
        }

  }
 } 
