pipeline {
    agent any

    stages {

        stage('Initialize') {
            steps {
                echo 'Starting Demo Pipeline'
            }
        }

        stage('Build') {
            steps {
                bat 'echo Building project'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Running tests'
            }
        }

        stage('Deploy') {
            steps {
                bat 'echo Deploying application'
            }
        }
    }

    post {
        always {
            echo 'Pipeline execution finished'
        }
    }
}
