pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building application...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }

        stage('post-Deployment') {
            steps {
                echo 'Deploying application...'
            }
        }

                stage('Trigger FS-1') {
            steps {
                build job: 'FS-1'
            }
        }
    }

    post {
        success {
            echo 'Pipeline PASSED successfully!'
        }

        failure {
            echo 'Pipeline FAILED!'
        }
    }
}