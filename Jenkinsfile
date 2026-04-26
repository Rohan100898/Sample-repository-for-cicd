pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/Rohan100898/Sample-Repos.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirement.txt'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'pytest'
            }
        }
    }
}