pipeline{
	agent any

	stages{
		stage ('clone'){
		
			steps{
				git 'https://github.com/vatsalkumarr/MavenDemoRepo.git'
				}
		}
		
		
		stage ('compile'){
		
			steps{
				
				
				 bat 'mvn clean install'
				
			}
		
		}
		}
		}
	
