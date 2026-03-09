pipeline {
    agent any

    tools {
        maven "Maven"
        jdk "JDK"
    }

    stages {

        stage('Initialize') {
            steps {
                echo "Starting Demo Pipeline..."
            }
        }

        stage('Build') {
            steps {
                bat 'mvn -version'
                echo "Build stage completed"
            }
        }

        stage('Test') {
            steps {
                echo "Running test stage..."
            }
        }

        stage('Deploy') {
            steps {
                echo "Deployment stage completed"
            }
        }
    }

    post {
        always {
            echo "Pipeline execution finished"
        }
        success {
            echo "Build Successful"
        }
        failure {
            echo "Build Failed"
        }
    }
}
