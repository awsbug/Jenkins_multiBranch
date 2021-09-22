node('master') 
{
    stage('Continuous Download_loans') 
	{

    git 'https://github.com/awsbug/maven.git'
	}
    stage('Continuous Build') 
	{
    sh label: '', script: 'mvn package'
	}
    stage('Continuous Deployment_loans') 
	{
sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war   ubuntu@:54.226.186.98/var/lib/tomcat9/webapps/qaenv.war'
	}


        

  



}
