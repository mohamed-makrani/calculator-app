pipeline {
    agent any

    tools {
        nodejs "node18"
    }

    stages {

        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'npm test'
            }
        }

        stage('Build') {
            steps {
                bat 'echo Build successful'
            }
        }

    }

    post {
        success {
            echo 'Bravo, déploiement réussi !'
        }
    }
}