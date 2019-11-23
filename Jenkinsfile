pipeline{
	agent any
	environment {
    		PATH = "C:\\Program Files\\Git\\usr\\bin;C:\\Program Files\\Git\\bin;${env.PATH}"
	}
	stages{
	        stage ('Clean') {
			steps {
				sh 'mvn clean'
	        	}
		}
	        stage ('Package') {
			steps {
	            		sh 'mvn package'
	        	}	
		}	
	}
		
	        
}
