pipeline {
    stages {
        def built_img
        
        stage('Clone repository') {
          checkout scm
        }

        stage('Build Docker image') {
          built_img = docker.build('./')
        }

        stage('Run Docker Container') {
          sh 'docker run -dp 3000:3000 docker-getting-started'
        }
    }
}
