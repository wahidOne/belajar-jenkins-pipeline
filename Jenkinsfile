pipeline {
    agent any

    stages {
        stage('Start') {
            steps {
                echo 'Starting the Pipeline...'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh("error 'Simulated Deployment Failure'") // Simulate a failure
            }
        }
        stage('Finish') {
            steps {
                echo 'Finishing the Pipeline...'
            }
        }
    }

    post {
        always {
            echo 'I Will Always say Hello.'
        }
        failure {
            echo 'I am sorry, the build failed.'
        }
        success {
            echo 'Yay! The build was successful.'
        }
        cleanup {
            echo 'Cleaning up after the build.'
        }
    }
}
