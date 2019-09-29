pipeline {
agent any

stages
{

stage "scm checkout" {
git credentialsId: 'ed4c5c22-12dd-4cac-ab0c-7b4729cc1bb1', url: 'https://github.com/Wasim-devops/maven-project.git'
}

}
{

stage ('Testing stage'){

stage{
withMaven(jdk: '', maven: 'Mavenlocal') 
{
    sh 'mvn test'
}
}
}
}
}
