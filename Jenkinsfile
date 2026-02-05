pipeline {
    agent any

    tools {
        maven 'maven-3.9.12'
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build with Maven') {
            steps {
                bat 'mvn clean compile'
            }
        }
    }
}