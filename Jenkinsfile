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
                bat 'python --version'
            }
        }

        stage('Test') {
            steps {
                bat 'python -m unittest test_app.py'
            }
        }

        stage('Deploy') {
            steps {
                bat 'echo App tested and ready to deploy!'
            }
        }
    }
}
