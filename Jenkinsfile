pipeline {
    agent any

    stages {
        stage('clean and compile') {
            steps {
                sh "mvn clean compile"
            }
        }
        stage('test'){
            steps{
                sh "mvn test"
            }
        }
        stage('package'){
            steps{
                sh "mvn package"
            }
        }
        stage('Archving'){
            steps{
                sh "archiveArtifacts '**/target/*.jar"
            }
        }
        
}

