pipeline {
    agent any
    tools {
        maven 'MAVEN_HOME'
    }
    stages {
        stage('Checkout Source') {
            steps {
                checkout scm
            }
        }
        stage('Verify Maven Version') {
            steps {
                bat "mvn -version"
            }
        }
        stage('Build Project') {
            steps {
                bat "mvn clean install"
            }
        }
        stage('Deploy Project') {
            steps {
                // Uncomment the following line if you want to use custom settings.xml for Maven authentication
                // bat "mvn clean deploy --settings C:\\Users\\Rutusoft\\.m2\\settings.xml"
                bat "mvn clean deploy"
            }
        }
    }
}
