node('master') 
{
    stage('Continuous Download') 
	{
    git 'https://github.com/sunildevops77/maven.git'
	}
    stage('Continuous Build') 
	{
    sh label: '', script: 'mvn package'
	}
    stage('Continuous Deployment') 
	{
sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/j1_loans/webapp/target/webapp.war   ubuntu@172.31.30.222:/var/lib/tomcat8/webapps/qaenv.war'
	}

}
