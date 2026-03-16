pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/Saurav2k05/demopipeline.git', branch: 'main'
            }
        }
        stage('Build') {
            steps {
                bat 'echo Building project...'
            }
        }
        stage('Test') {
            steps {
                bat 'echo Running tests...'
            }
        }
        stage('Deploy') {
            steps {
                bat 'echo Deploying...'
            }
        }
    }
}
