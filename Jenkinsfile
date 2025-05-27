pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/loki346/Devo.git'
            }
        }

        stage('Install Python') {
            steps {
                bat '''
                    python --version
                    python -m pip install --upgrade pip
                '''
            }
        }

        stage('Run Script') {
            steps {
                bat 'python main.py'
            }
        }
    }
}
