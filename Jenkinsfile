pipeline {
    agent any

    tools {
        maven 'MAVEN'
    }

    stages {

        stage('Checkout Code') {
            steps {
                git 'https://github.com/example/selenium-project.git'
            }
        }

        stage('Build Project') {
            steps {
                sh 'mvn clean compile'
            }
        }

        stage('Run Selenium Tests') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Archive Results') {
            steps {
                junit 'target/surefire-reports/*.xml'
            }
        }
    }
}
