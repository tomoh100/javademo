pipeline {
         agent { label "agent01" } 
	tools {
        maven 'Maven 3.9.8' // This should match the name given in Global Tool Configuration
    }
		 stages{ 
		 
		         stage("Build package"){
			   steps{
				   script {
			       sh " mvn --version " 
				   }
			   }
				}
			   stage ("build notification"){
			   steps{
			        echo " this build is completed " 
					}
			    }	 
		 }
  post{
    always{
           cleanWs()
    }
  }
}
