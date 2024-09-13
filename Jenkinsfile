pipeline {
    agent any
    tools {
        maven 'MAVEN_HOME'
    }
    stages {
        stage('Build Maven') {
            steps {
                checkout scm
                sh 'mvn clean install'
            }
        }
}