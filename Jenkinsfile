pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from the repository
                git 'https://github.com/your-repo/your-project.git'
            }
        }
        stage('Build') {
            steps {
                // Build the project
                sh './gradlew build'
            }
        }
        stage('Test') {
            steps {
                // Run tests
                sh './gradlew test'
            }
        }
        stage('Deploy') {
            steps {
                // Deploy the application
                sh './deploy.sh'
            }
        }
    }
}

