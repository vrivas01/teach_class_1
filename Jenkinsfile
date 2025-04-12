pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'javac -d target ContarLetras.java'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'java -cp target ContarLetras "Prueba ejecución de java"'
            }
        }
    }
}