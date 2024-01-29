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
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/Sanchita57/Demo_app1.git'
            }
        }
    }   
}
