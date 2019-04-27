pipeline {
         agent any
         stages {
             stage('Preparation') {
               steps {
		       sh "mvn clean -f springExample"
		             }     
                            }
	     stage('Test') {
               steps {
			   sh "mvn test -f springExample"
		             }  
                        }
	     stage('Build') {
               steps {
               sh "mvn package -f springExample"
		             }
			             }
                 }
        }
