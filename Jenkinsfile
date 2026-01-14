pipeline {
    agent any

    tools {
        nodejs "Node25"
        dockerTool "Dockertool" 
    }

    stages {
        stage('Instalar dependencias') {
            steps {
                sh 'npm install'
            }
        }

        stage('Ejecutar tests') {
            steps {
                sh 'npm test'
            }
        }
    }
}