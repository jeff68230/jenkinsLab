pipeline {
    agent any
    environment {
        APP_NAME = 'my-app'
    }
    stages {
        stage('Build') {
            steps {
                script {
                    def buildVersion = "1.0.${env.BUILD_NUMBER}"
                    echo "Building ${APP_NAME} version ${buildVersion}"
                }
            }
        }
        stage('Test') {
            steps {
                echo "Testing ${APP_NAME}..."
            }
        }
        stage('Deploy') {
            steps {
                script {
                    def buildVersion = "1.0.${env.BUILD_NUMBER}"
                    echo "Deploying ${APP_NAME} version ${buildVersion}"
                }
            }
        }
    }
}
