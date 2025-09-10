pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo "Building code using Maven"
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo "Running tests using Selenium"
            }
        }
        stage('Code Analysis') {
            steps {
                echo "Analysing code using SonarQube"
            }
        }
        stage('Security Scan') {
            steps {
                echo "Running security scan's using Jenkins' integrated Security Scanner (CodeQL)"
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo "Deploying application to AWS EC2 staging server"
            }
        }
        stage("Integration Tests on Staging") {
            steps {
                echo "Running integration tests on staging server using JUnit 5"
            }
        }
        stage("Deploy to Production") {
            steps {
                echo "Deploying application to AWS EC2 production server"
            }
        }
    }
}