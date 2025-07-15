pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/rafeekca/python-cicd-demo.git'
            }
        }

        stage('Install Python') {
            steps {
                sh 'python3 --version'
            }
        }

        stage('Test') {
            steps {
                sh 'python3 -m unittest test_app.py'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "App tested and ready to deploy!"'
            }
        }
    }
}
