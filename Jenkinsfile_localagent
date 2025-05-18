pipeline {
    agent any

    triggers {
        pollSCM('*/5 * * * *')  // Poll SCM every 5 minutes
    }

    stages {
        stage('Build') {
            steps {
                echo "Building..."
                sh '''
                    echo "Building from Jenkins pipeline"
                '''
            }
        }

        stage('Test') {
            steps {
                echo "Testing..."
                sh '''
                    echo "Testing the build triggered from Jenkins pipeline."
                '''
            }
        }

        stage('Deliver') {
            steps {
                echo "Delivering..."
                sh '''
                    echo "Performing delivery steps."
                '''
            }
        }
    }
}
