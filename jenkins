pipeline {
  agent any 
    tools {
       //Installed the maven version configured as 'M3' and add it to the path
     jdk 'Java 8'
     maven 'Maven-3.3.9'
  }
  
  stages 
  {
   stage('checkout') {
     steps {
       // get some code from a GitHub repository
       git 'https://github.com/madhupriya1121/game-of-life.git'
    }
  }
  stage('compile and build') {
      steps {
          sh '''
          mvn clean install -U -Dmaven.skip.test=true
          '''
      }
  }
}
}
