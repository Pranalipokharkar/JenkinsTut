pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from source control
                git branch: 'main', url: 'https://github.com/Pranalipokharkar/JenkinsTut.git'
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
