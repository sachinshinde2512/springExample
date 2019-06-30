pipeline {
         agent any
         stages {
             stage('Preparation') {
               steps {
		       echo "Cleaning the Workspace ............"
		       sh "mvn clean"
		             }     
                            }
             stage('Compile') {
               steps {
		       echo "Compile from Source............"
		       sh "mvn compile"
		             }     
                            }
	     stage('Test') {
               steps {
		       	   echo "Test the build ........."
			   sh "mvn test"
		             }  
                        }
	     stage('Build') {
               steps {
	       echo "Packaging the build ........."
               sh "mvn package"
		             }
			             }
                 }
        }
