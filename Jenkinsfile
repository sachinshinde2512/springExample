pipeline {
         agent any
         stages {
             stage('Preparation') {
               steps {
		       sh "mvn clean"
		             }     
                            }
	     stage('Test') {
               steps {
			   sh "mvn test"
		             }  
                        }
	     stage('Build') {
               steps {
               sh "mvn package"
		             }
			             }
                 }
        }
