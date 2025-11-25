pipeline {
    agent any

    stages {
        stage('git clone') {
            steps {
               //bat rmi /s /q MavenJavaDemo
               bat "git clone https://github.com/Sai-Rohan005/SELabinternal2.git"
               bat "mvn clean -f MavenJavaDemo"
            }
        }
        stage('install') {
            steps {
               bat "mvn install -f MavenJavaDemo"
            }
        }
        stage('test'){
            steps{
                bat "mvn test -f MavenJavaDemo"
            }
            
        }
    }
}
