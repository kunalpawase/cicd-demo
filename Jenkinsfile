pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat '"C:\\Users\\kunal\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe" app.py'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat '"C:\\Users\\kunal\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe" -m pip install -r requirements.txt'
            }
        }

        stage('Test') {
            steps {
                bat '"C:\\Users\\kunal\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe" -m pytest'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment successful'
            }
        }
    }
}