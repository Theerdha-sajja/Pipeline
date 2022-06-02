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
			enviroment{
				PATH = " D:\DevOps_softwares\apache-maven-3.8.5\bin:$PATH"
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
