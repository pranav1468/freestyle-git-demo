pipeline {
    agent any

    triggers {
        // Poll SCM every 2 minutes 
        pollSCM('H/2 * * * *')
    }

    stages {
        stage('Checkout') {
            steps {
                echo "Checking out code from GitHub branch b1..."
            }
        }

        stage('Build') {
            steps {
                echo "Building the project..."
                echo "Change made to test SCM trigger"
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying application..."
            }
        }
    }
}
