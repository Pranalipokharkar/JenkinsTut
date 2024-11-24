pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from source control
                git branch: 'main', url: 'https://github.com/your-repo/java-maven-project.git'
            }
        }
        stage('Setup Maven') {
            steps {
                // Ensure Maven is installed
                sh 'mvn --version'
            }
        }
        stage('Build') {
            steps {
                // Build the project using Maven
                sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                // Run tests
                sh 'mvn test'
            }
        }
        
    }

}
