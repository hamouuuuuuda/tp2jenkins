pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Example: sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Example: sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Example: sh 'kubectl apply -f deployment.yaml'
            }
        }
    }

    post {
        always {
            echo 'Pipeline completed.'
        }
    }
}
