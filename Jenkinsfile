pipeline {
    agent any

    tools {
        maven 'MAVEN'
    }

    stages {

        stage('Checkout Code') {
            steps {
                git 'https://github.com/Saurav2k05/demopipeline.git'
            }
        }

        stage('Build Project') {
            steps {
                bat 'mvn clean install'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'mvn test'
            }
        }
    }
}
