pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application'
            }
        }
    }

    post {
        success {
            echo 'All tests passed. Safe to deploy.'
        }
        failure {
            echo 'Tests failed. Deployment stopped.'
        }
    }
}
