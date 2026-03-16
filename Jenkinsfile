pipeline {
    agent any

    tools {
        maven 'MAVEN'
    }

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/Saurav2k05/demopipeline.git'
            }
        }

        stage('Build Project') {
            steps {
                dir('your-maven-folder') { // Replace with actual folder if pom.xml is not at root
                    bat 'mvn clean install'
                }
            }
        }

        stage('Run Tests') {
            steps {
                dir('your-maven-folder') {
                    bat 'mvn test'
                }
            }
        }

    }
}
