pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh "export PATH=$PATH:/usr/local/jdk1.8.0_161/bin:/usr/local/jdk1.8.0_161/jre/bin:/usr/local/apache-ant-1.10.2/bin; /usr/local/apache-ant-1.10.2/bin/ant"
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

