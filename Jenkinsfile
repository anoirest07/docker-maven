node{
	        
	        stage ('SCM Checkout') {
	            git 'https://github.com/anoirest07/docker-maven-spring.git'
	        }
	        
	        stage ('Compile-Package') {
	            def mvnHome = tool name: 'Maven 3.6.2', type: 'maven'
	            sh "${mvnHome}/bin/mvn package"
	        }
	        
}
