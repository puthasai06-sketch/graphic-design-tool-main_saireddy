pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/puthasai06-sketch/graphic-design-tool-main_saireddy.git'
            }
        }

        stage('Build and Deploy') {
            steps {
                sh 'docker compose down'
                sh 'docker compose up -d --build'
            }
        }

    }
}
