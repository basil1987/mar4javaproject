pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh "ant"
            }
        }
        stage('Test') { 
            steps {
                sh "echo TESTING"
            }
        }
        stage('Deploy') { 
            steps {
                sh "cp **/*.war /usr/local/apache-tomcat-7.0.85/webapps"
            }
        }
    }
}

