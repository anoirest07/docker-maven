node{
	        
	        stage ('mvn clean') {
	            
	            sh 'mvn  clea'
	        }
	        
	        stage ('mvn package') {
	            
	            sh 'mvn  package'
	        }
	        stage ('Build Docker Image'){
	            sh 'mvn docker:build'
	        }
}
