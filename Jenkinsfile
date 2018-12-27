pipeline {
    agent any 
    stages {
        stage('Clone and Clean') { 
            steps {
                sh "/usr/local/src/apache-maven/bin/mvn clean"
            }
        }
        stage('Test') { 
            steps {
                sh "/usr/local/src/apache-maven/bin/mvn test"
            }
        }
        stage('Deploy') { 
            steps {
                sh "/usr/local/src/apache-maven/bin/mvn package"
            }
        }
    }
}
