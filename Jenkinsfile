pipeline 
{
  agent any
  stages 
  {
    stage('scm checkout') {
      steps
       {
        git branch: 'master', url: 'https://github.com/Ajinkya787/maven-project_Ajinkya.git'
      }
    }

   stage('code compile')
 {
  steps 
  { 
    withMaven(globalMavenSettingsConfig: '', jdk: 'JDK_HOME', maven: 'MAVEN_HOME', mavenSettingsConfig: '', traceability: true) {
     sh 'mvn compile'
}
 }
 }
}
}







