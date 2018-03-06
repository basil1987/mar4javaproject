pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh "/usr/local/apache-ant-1.10.2/bin/ant"
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

