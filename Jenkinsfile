pipeline {
    agent {
        docker { image 'node:18-alpine' }
    }
    stages {
        stage('Pobieranie kodu') {
            steps {
                checkout scm
            }
        }
        stage('Test wewnątrz kontenera') {
            steps {
                sh 'node --version'
                sh 'ls -la'
                echo 'Testy zakończone sukcesem!'
            }
        }
    }
}
