pipeline {
    agent any

    triggers {
        pollSCM('H/15 * * * *')
    }

    stages {

        stage('Build') {
            steps {
                echo 'Building project using Maven'
            }
        }

        stage('Unit & Integration Tests') {
            steps {
                echo 'Running tests using JUnit & Selenium'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Analyzing code using SonarQube'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Scanning using OWASP ZAP'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Deploying to AWS EC2 staging server'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Running staging tests using Postman'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Deploying to production server'
            }
        }
    }
}
