pipeline {
    agent any

    stages {
        stage('Build & Deploy') {
            steps {
                echo 'Starting build and deploy scripts...'
                sh 'chmod +x build.sh && ./build.sh'
                sh 'chmod +x deploy.sh && ./deploy.sh'
            }
        }
    }

    post {
        success {
            echo '✅ Build and deployment completed successfully.'
        }
        failure {
            echo '❌ Build or deployment failed.'
        }
    }
}
