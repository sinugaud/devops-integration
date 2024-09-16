pipeline {
    agent any
    tools {
        maven 'MAVEN_HOME'
    }
    stages {
        stage('Build Maven') {
            steps {
                checkout scm
                sh "mvn -version"
                sh 'mvn clean install'
            }
     }   }
}

git branch: 'main', credentialsId: 'login', url: 'https://github.com/sinugaud/devops-integration'