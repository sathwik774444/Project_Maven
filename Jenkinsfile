pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building application'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests'
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
            echo 'Pipeline SUCCESS'
        }
        failure {
            echo 'Pipeline FAILED'
        }
    }
}
