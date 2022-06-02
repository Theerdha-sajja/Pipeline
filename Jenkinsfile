pipeline{
		agent any
		stages{
		       stage('one'){
					steps{
					       echo "Hello Theerdha"
						sh 'git clone https://github.com/Theerdha-sajja/Pipeline.git'
					      }
				    }
                      stage('two'){
                                   steps{
                                   input('do you want to proceed?')
                                 }
                            }
		       stage('three'){
					steps{
					       sh 'mvn validate'
					      }
				     }
		       stage('four'){
					 steps{
					        sh 'mvn compile'
					      }
				    }							
		       stage('five'){
					 steps{
					        sh 'mvn package'
					      }
                			}
			   }
	    }
