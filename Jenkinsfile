pipeline {
    agent any
    tools {
        maven 'M3'
    }
    stages {
        stage('Test Maven') {
            steps {
                bat 'mvn --version'
            }
        }
    }
}