pipeline{
	agent any

	stages{
		stage ('clone'){
		
			   steps{
				git 'https://github.com/vatsalkumarr/EMS.git/'
				}
	                       }
		
		
		stage ('compile'){
		
				steps{		
				 	bat 'mvn clean install'
				      }
		
				}
		
	      stage('SonarQube analysis') { 
		      
		      steps{
			      bat 'sonar-scanner -Dsonar.projectKey=EMS_Master ' +
				       '-Dsonar.projectName=EMS_Master ' +
	  	  '-Dsonar.projectVersion=1.0 ' +
		 '-Dsonar.sources=src ' +
	 	 '-Dsonar.java.binaries=target/classes ' +
         	 '-Dsonar.login=admin ' +
         	 '-Dsonar.password=admin123 ' 
		      }
                 
          				}
           }
 }
	
