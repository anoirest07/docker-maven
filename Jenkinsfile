pipeline {
    agent none
   stages {     
    stage('Maven Install') {
      agent {         
       docker {          
         image 'maven:alpine'
         args '-v /root/.m2:/root/.m2'      
     }       
  }       
  steps {
       sh 'mvn clean install'
       }
     }
   }
 }
