pipeline{
  
    agent {
    label "windows"
  }
  tools {
    maven 'Maven 3.1.1'
    jdk 'java8'
  }
  stages {
   
    stage ('Initialize'){
      steps {
        bat 
        echo "PATH = %PATH%
        echo "M2_HOME = %M2_HOME%"
      }
    }
    
    stage ('Build'){
      steps {
        bat 'mvn install'
        }
    }
    
    
  }
}

