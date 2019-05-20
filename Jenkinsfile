pipeline {
    agent any 
    stages {
        stage('clean') { 
            steps {
                sh "mvn clean"
            }
        }
        stage('compile') { 
            steps {
                sh "mvn compile"
            }
        }
        stage('Deploy') { 
            steps {
                sh "mvn test"
            }
            stage('Package') { 
            steps {
                sh "mvn package"
            }
        }
    }
}
