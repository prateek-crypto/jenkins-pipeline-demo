pipeline {
    agent any

    parameters {
        string(name: 'USER_NAME', defaultValue: 'Prateek', description: 'Enter your name')
        choice(name: 'ENV', choices: ['dev', 'prod'], description: 'Select environment')
    }

    stages {

        stage('Build') {
            steps {
                echo "Hello ${params.USER_NAME}"
                sh 'echo Running application...'
            }
        }

        stage('Long Running Task') {
            steps {
                echo "Simulating long task..."
                sh 'sleep 30'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying to ${params.ENV}"
            }
        }
    }
}
