pipeline {
    agent any
    stages {
        stage('Build Image') {
            steps {
                sh 'docker build -t my-app:latest .'
            }
        }
        stage('Test Run') {
            steps {
                sh 'docker run --rm my-app:latest echo "Success!"'
            }
        }
    }
}