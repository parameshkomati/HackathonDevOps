pipeline{
  
    agent {
    label "windows"
  }
  tools {
    maven 'MAVEN_HOME'
    jdk 'JAVA_HOME'
  stages {
   
    stage ('Initialize'){
      steps {
        bat 
        echo "PATH = %PATH%"
        echo "M2_HOME = %MAVEN_HOME%"
      }
    }
    
    stage ('Build'){
      steps {
        bat 'mvn install'
        }
    }
    
    
  }
}

