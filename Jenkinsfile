pipeline {
  environment {
    registry = "pratush43/dock"
    registryCredential = 'dockerhub'
  }
  agent none
    stages {
        stage('Build') {
          agent {
    node{
    label 'micro2'
    } 
  }
          
            steps {
              dir("dotnet-core-hello-world"){
              sh 'cd Core_HelloWorld'
              sh 'pwd'
              sh 'ls -lrt'
              
                sh 'dotnet build'
                
            }
            }
        }
        
    }
      
}
