pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                // e.g., using Maven
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Running Unit and Integration Tests...'
                // e.g., JUnit
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Analyzing the Code...'
                // e.g., SonarQube
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Running Security Scan...'
                // e.g., OWASP Dependency-Check
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Deploying to Staging...'
                // e.g., AWS EC2 deployment
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Running Integration Tests on Staging...'
                // e.g., Integration test script
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Deploying to Production...'
                // e.g., Deploy to Production server
            }
        }
    }
    post {
        success {
            mail to: 'nathashaliyanage96@gmail.com',
                 subject: "Pipeline Success",
                 body: "The pipeline has completed successfully."
        }
        failure {
            mail to: 'nathashaliyanage96@gmail.com',
                 subject: "Pipeline Failure",
                 body: "The pipeline has failed. Check Jenkins logs for details."
        }
    }
}
