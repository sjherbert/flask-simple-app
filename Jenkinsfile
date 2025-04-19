pipeline {
    agent any
    stages {
        stage('Clone Repo') {
            steps {
                git clone 'https://github.com/sjherbert/flask-simple-app.git'
            }
        }
        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }
        stage('Run Flask App') {
            steps {
                sh 'python app.py &'
            }
        }
    }
}
