pipeline {
    agent any
    stages {
        stage('---clean---') {
            steps {
                withmaven('maven:m3') { 
                sh "mvn clean"
                }
            }
        }
        stage('--test--') {
            steps {
                withmaven('maven:m3') { 
                sh "mvn test"
                }
            }
        }
        stage('--package--') {
            steps {
                withmaven('maven:m3') { 
                sh "mvn package"
            }
        }
    }
}
