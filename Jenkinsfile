pipeline {
    agent any
    stages {
        stage ('SCM Checkout') {
            steps { 
   git credentialsId: 'ed4c5c22-12dd-4cac-ab0c-7b4729cc1bb1', url: 'https://github.com/Wasim-devops/maven-project.git'
      }
        }
        stage ('Code Test') {
    steps
  {
   withMaven(maven: 'Mavenlocal')
  {
    sh 'mvn test'
  }
 } 
 
}
}
}
