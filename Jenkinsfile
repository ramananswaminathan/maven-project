pipeline {
    agent any
    tools {
    maven 'M3'
   }
    stages{
        stage('Build'){
            steps {
             sh 'mvn clean package'
            }
            post {
                success {
                    echo 'Now Archiving...'
                    archiveArtifacts artifacts: '**/target/*.war'
                }
            }
        }
    
        stage('Deploy Staging') {
   	  steps {
		   build job: 'deploy-to-staging'
		}
	  }	
	}
}

