node{
	        stage ('git checkout'){
	            url: 'https://github.com/anoirest07/docker-maven-spring.git'
	        }
	        stage ('mvn clean') {
	            def mvnHome = tool name: 'Maven 3.6.2', type: 'maven'
	            def mvnCMD = "${mvnHome}/bin/mvn"
	            sh "${mvnCMD}  clean"
	        }
	        
	        stage ('mvn package') {
	            def mvnHome = tool name: 'Maven 3.6.2', type: 'maven'
	            def mvnCMD = "${mvnHome}/bin/mvn"
	            sh "${mvnCMD}  package"
	        }
	        stage ('Build Docker Image'){
	            sh 'mvn docker:build'
	        }
}
