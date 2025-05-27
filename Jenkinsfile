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
                sh 'python3 --version'
                sh 'pip3 install --upgrade pip'
            }
        }

        stage('Run Script') {
            steps {
                sh 'python3 main.py'
            }
        }
    }
}
