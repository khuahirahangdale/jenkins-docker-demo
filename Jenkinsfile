
pipeline {
    agent any

    stages {
        stage('Check Docker') {
            steps {
                sh 'docker --version'
            }
        }

        stage('Build Image') {
            steps {
                sh 'docker build -t my-python-app:v1 .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run --rm my-python-app:v1'
            }
        }
    }
}
