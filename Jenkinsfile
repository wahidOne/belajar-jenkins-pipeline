pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
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
