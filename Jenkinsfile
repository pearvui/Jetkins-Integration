pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building application and environment using Maven'
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Running Selenium tests on Unit and Intergration'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Running SonarQube analysis'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Running OWASP Security Dependency Scan Check'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Deploying to AWS EC2 staging server'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Running Cypress tests on staging'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Deploying application to production server using SSH'
            }
        }
    }
}