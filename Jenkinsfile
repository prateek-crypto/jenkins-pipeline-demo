pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo "Fetching code from GitHub..."
                git 'https://github.com/YOUR-USERNAME/jenkins-pipeline-demo.git'
            }
        }

        stage('Build') {
            steps {
                echo "Running Python app..."
                sh 'python3 app.py'
            }
        }

        stage('Done') {
            steps {
                echo "Pipeline completed successfully"
            }
        }
    }
}
