pipeline{
	agent any
	stages{
	        stage ('Clean') {
			steps {
				sh 'mvn clean'
	        	}
		}
	        stage ('CPackage') {
			steps {
	            		sh 'mvn package'
	        	}	
		}	
	}
		
	        
}
