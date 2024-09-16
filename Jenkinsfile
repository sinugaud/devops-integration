pipeline {
    agent any
    tools {
        maven 'MAVEN_HOME'
    }
    stages {
        stage('Build Maven') {
            steps {
                checkout scm
                bat "mvn -version"
                bat "mvn clean install"
                bat "mvn clean deploy --settings C:\\Users\\Rutusoft\\.m2\\settings.xml"
            }
     }   }
}

// git branch: 'main', credentialsId: 'login', url: 'https://github.com/sinugaud/devops-integration'