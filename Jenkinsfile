pipeline{
	agent any
	tools {
		maven 'maven 3.6.2'
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
				bat 'mvn clean'
	        	}
		}
	        stage ('Package') {
			steps {
	            		bat 'mvn package'
	        	}	
		}	
	}
		
	        
}
