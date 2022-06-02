pipeline{
		agent any
		stages{
		       stage('one'){
					steps{
					       echo "Hello Theerdha"
					      }
				    }
                      stage('two'){
                                   steps{
                                   input('do you want to proceed?')
                                 }
                            }
		       stage('three'){
					steps{
					       mvn validate
					      }
				     }
		       stage('four'){
					 steps{
					        mvn compile
					      }
				    }							
		       stage('five'){
					 steps{
					        mvn package
					      }
                			}
			   }
	    }
