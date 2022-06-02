pipeline{
		agent any
	        tools {
       		         maven "MAVEN"
                         jdk "JAVA"
                      }
                stages {
                       stage('Initialize'){
                       steps{
                             echo "PATH = ${MAVEN_HOME}/bin:${PATH}"
                             //echo "M2_HOME = /opt/maven"
                            }
                          }
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
