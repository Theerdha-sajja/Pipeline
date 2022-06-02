pipeline{
		agent any
	stages{
		       stage('three'){
					steps{
						//bat "git clone   https://github.com/Theerdha-sajja/Pipeline.git"
					        bat "mvn validate"
					      }
				     }
		       stage('four'){
					 steps{
					        bat "mvn compile"
					      }
				    }							
		       stage('five'){
					 steps{
					        bat "mvn package"
					      }
                			}
			   }
	    }
