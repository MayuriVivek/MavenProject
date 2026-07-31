pipeline {  
  agent any
 environment {
        PATH = "/opt/maven/bin:$PATH"
    }   
 stages{
       stage('building'){
	steps{
	sh 'mvn clean package'
           } 
	}
	stage('pipeline completed'){
	steps{
	echo 'pipeline completed'
           } 
        }






          }
        }
      
