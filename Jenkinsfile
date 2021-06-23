pipeline {
 
  agent any

  stages {
    stage('Cloning Git') {
      steps {
        git branch: 'main', credentialsId: 'brijesh2311', url: 'https://github.com/brijesh2311/python.git'
      }
    }
  }
  
}
