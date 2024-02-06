pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building the Java application'
                sh 'javac Main.java'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests'
                sh 'java Main'
            }
        }
    }
    
    post {
        always {
            sh 'rm Main.class'
        }
    }
}
