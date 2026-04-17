pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo "Checking out code..."
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "Running build stage..."
            }
        }

        stage('SonarQube Scan') {
            steps {
                echo "SonarQube scan will run here"
            }
        }

        stage('Snyk Scan') {
            steps {
                sh 'snyk test || true'
            }
        }
    }
}
