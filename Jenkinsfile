pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/your-username/your-repo.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                // For example, if it's Java:
                // sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // For example:
                // sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
                // Add deploy commands here
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished.'
        }
    }
}
