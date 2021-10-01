pipeline {
    agent any
	
	  tools
    {
       maven "maven"
    }
 stages {
      stage('checkout') {
           steps {
             
                git branch: 'master', url: 'https://github.com/hassnain421/CICD-using-docker.git'
             
          }
        }
	 stage('Execute Maven') {
           steps {
		   sh 'mvn clean package'             
	   }
        }
        
	}
