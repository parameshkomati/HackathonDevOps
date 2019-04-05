pipeline{
  
    agent {
    label "windows"
  }
  tools {
    //echo 'Pipile script ::'
    maven 'maven3'
    jdk 'java8'
  }
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
}

