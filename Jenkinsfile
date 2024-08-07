pipeline {
         agent { label "agent01" } 
		 stages{ 
		 
		         stage("Build package"){
			   steps{
			       sh " mvn -version " 
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
