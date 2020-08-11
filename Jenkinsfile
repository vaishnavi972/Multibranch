node('master') 
{
  stage('ContinuousDownload_Loans') 
  {
      git 'https://github.com/vaishnavi972/maven.git'
  }  
  stage('ContinuousBuild_Loans') 
  {
      sh label: '', script: 'mvn package'
  }  
} 
