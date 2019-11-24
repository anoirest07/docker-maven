pipeline{
	agent any
	tools {
		maven 'Maven 3.6.2'
	}
	stages{
		stage ('Initialize') {
			steps{
			bat ''' 
				echo "PATH=${PATH}"
				echo "M2_HOME = ${M2_HOME}"
				'''
			}
		}
	        stage ('Clean') {
			steps {
				bat 'mvn clean -s C:/Users/anoir/.m2/settings.xml'
	        	}
		}
	        stage ('Package') {
			steps {
	            		bat 'mvn package -s C:/Users/anoir/.m2/settings.xml'
	        	}	
		}	
	}
		
	        
}
