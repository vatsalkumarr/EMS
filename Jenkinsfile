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
		}
		}
	
