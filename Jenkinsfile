pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "🔥 Build Stage"
                sh 'echo Building source...'
            }
        }

        stage('Test') {
            steps {
                echo "🧪 Test Stage"
                sh 'echo Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo "🚀 Deploy Stage"
                sh 'echo Deploying application...'
            }
        }
    }
}
