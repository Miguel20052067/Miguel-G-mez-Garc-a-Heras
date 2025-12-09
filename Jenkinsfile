pipeline {
    agent any

    stages {
        stage('Checkout'){
            steps { 
                checkout scm 
            }
        }
        stage('Build'){
            steps{ 
                bat 'echo "Build ejecutado"' 
            }
        }
        stage('Archive'){
            steps{ 
                archiveArtifacts artifacts: '**/*' 
            }
        }
        stage('Deploy'){
            steps{ 
                bat 'echo "Desplegando..."' 
            }
        }
    }
}


