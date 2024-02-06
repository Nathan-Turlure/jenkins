pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building the Java application'
                // Ici, vous pouvez ajouter des étapes de construction Java si nécessaire
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests'
                sh 'javac Main.java' // Compile Java file
                sh 'java Main' // Run Java program
                // Ici, vous pouvez ajouter des étapes de test supplémentaires si nécessaire
            }
        }
    }
    
    post {
        always {
            echo 'Cleaning up'
            sh 'rm Main.class' // Supprimer le fichier de classe Java après l'exécution
            // Ajoutez d'autres actions de nettoyage ici si nécessaire
        }
    }
}
