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
                sh '''
                 mkdir -p /var/www/html/test

                # Jenkins 워크스페이스에서 결과물 복사
                 cp -r * /var/www/html/test/

                echo "배포 완료!"
                '''
            }
        }
    }
}
