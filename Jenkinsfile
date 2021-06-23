pipeline {
 
 environment {
registry = "brijesh2328/mypython"
registryCredential = 'docker_hub'
dockerImage = ''
}
 
 agent any
   
 
  stages {
    stage('Cloning Git') {
      steps {
        git branch: 'main', credentialsId: 'brijesh2311', url: 'https://github.com/brijesh2311/python.git'
      }
    }
  
 
 stage('Building our image') {
   steps{
    script {
      dockerImage = docker.build registry + ":$BUILD_NUMBER"
      }
   }
 }
 
 
  }
  
}
