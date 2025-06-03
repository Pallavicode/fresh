pipeline {
    agent any

    environment {
        DOCKER_IMAGE = "pallavidocker2024/pallavidocker2024"}

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/Pallavicode/fresh.git'  }
        } 

  stage('Build') {
            steps {
                sh 'chmod +x build.sh && ./build.sh'
            }
        }
    }
}

