pipeline 
{
  agent any
  stages {
    stage('scm checkout') {
      steps {
        git branch: 'master', url: 'https://github.com/Ajinkya787/maven-project_Ajinkya.git'
      }
    }

    stage('code validate') //validate then compile
    {
      steps {
        withMaven(globalMavenSettingsConfig: '', jdk: 'JAVA_HOME', maven: 'MAVEN_HOME', mavenSettingsConfig: '', traceability: true) {
          sh 'mvn validate'
        }
      }
    }
  }}




