pipeline
 {
  agent any 
  
   tools { 
        maven 'maven3.6.3' 
        jdk 'java8' 
    }
  
  stages {
    stage('Build Application') {
    steps {
    sh 'mvn clean install'
     } 
    }
  
  
  stage('Deploy Application To Mulesoft CloudHub') {
  steps {
    sh 'mvn package deploy -DmuleDeploy'
   }
  }
  
  }
 }