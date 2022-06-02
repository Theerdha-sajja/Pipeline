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
		       stage('three'){
					steps{
						bat "git clone   https://github.com/Theerdha-sajja/Pipeline.git"
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
