pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/shatskiy-O/sdvps-materials'
            }
        }

        stage('Test') {
            steps {
                sh 'go test .'
            }
        }

        stage('Build') {
            steps {
                sh 'docker build -t my-go-app .'
            }
        }
    }
}
