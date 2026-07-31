pipeline {  
  agent any
    stages{
       stage('cloning git repo') {
        steps{
	  git url: 'https://github.com/MayuriVivek/MavenProject.git' , branch: 'main'
             }
	}
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
       }
