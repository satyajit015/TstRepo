pipeline {
    agent any 
    stages {
        stage('Init') { 
            steps {
                powershell "write-host 'Say Helo Powershell' "                
            }
        }
        stage('Build') { 
            steps {                
                bat 'mvn clean'
                bat 'mvn test'
                bat 'mvn package'
            }
        }
        stage('Test') { 
            steps {
                bat 'echo test' 
            }
        }
        stage('Deploy') { 
            steps {
                bat 'echo package'
            }
        }
    }
}
