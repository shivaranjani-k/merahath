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
                sh "compile"
            }
        }
        stage('Deploy') { 
            steps {
                sh "test"
            }
            stage('Package') { 
            steps {
                sh "package"
            }
        }
    }
}
