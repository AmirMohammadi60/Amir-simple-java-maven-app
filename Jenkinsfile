pipeline {
    agent any
    environment {
     VERSION = 1.0
    }
    stages {
        stage('Build') {
            steps {
                echo 'Die Anwendung wird gebaut'
                sh '/opt/apache-maven-3.8.7/bin/mvn package'
            }
        }
        stage('Test') {
            steps {
                echo 'Die Anwendung wird getestet'
                sh '/opt/apache-maven-3.8.7/bin/mvn test'
            }
        }
    }
}
