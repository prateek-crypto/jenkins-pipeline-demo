pipeline {
    agent any

    stages {

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
