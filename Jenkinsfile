pipeline {
    agent any
    tools {
      maven 'MAVEN3'
      //jdk 'JDK8'
      //jfrog 'cli'         
    }
    stages {
        stage ('Checkout') {
            steps {
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/chocolate-riya/Demo_app1.git'
            }
        }
        stage ('Build') {
            steps {        
                sh 'mvn clean install'
                sh 'mvn package'
                sh 'cp ./target/*.jar ./'
                sh 'pwd'
                //sh 'docker images'
            }
        }
    }   
}
