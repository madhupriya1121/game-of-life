pipeline {
  agent any 
    tools {
       //Installed the maven version configured as 'M3' and add it to the path
     jdk 'Java8'
     maven 'Maven3.3.9'
  }
  
  stages 
  {
   stage('checkout') {
     steps {
       // get some code from a GitHub repository
       git 'https://github.com/madhupriya1121/game-of-life.git'
    }
  }
}
}
