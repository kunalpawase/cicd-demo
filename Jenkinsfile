pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'py app.py'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'py -m pip install -r requirements.txt'
            }
        }

        stage('Test') {
            steps {
                bat 'py -m pytest'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment successful'
            }
        }
    }
}