node('master') 
{
  stage('ContinuousDownload_Master') 
  {
      git 'https://github.com/vaishnavi972/maven.git'
  }  
  stage('ContinuousBuild_Master') 
  {
      sh label: '', script: 'mvn package'
  }  
  stage('ContinuousDeployment_Master') 
  {
      sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war ubuntu@172.31.5.113:/var/lib/tomcat8/webapps/testapp.war'
  } 
