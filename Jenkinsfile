pipeline{
   agent any
   environment{
       PATH= "/opt/maven/bin:$PATH"   
   }  
   stages{
       stage('Git cloning'){
         steps{
	   git url: 'https://github.com/MayuriVivek/MavenProject.git', branch:'main'
         }
       }
       stage('building war file'){
	steps{
         sh 'mvn clean package'
         }
	}
       stage('storing artifact in jenkins'){
	steps{
	archiveArtifacts artifact : 'target/*.war'
         }
       }
    }
   post{
   always {echo "pipeline is running" }
   success {echo "successfully completed"}
   failure { echo " Failed"}
   }
}
      
