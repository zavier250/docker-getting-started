pipeline {
    agent any
    
    stages {
        stage('Build Docker image') {
            steps {
                sh 'sudo docker build -t docker-getting-started .'
            }
        }

        stage('Run Docker Container') {
            steps {
                sh 'sudo docker run -dp 3000:3000 docker-getting-started'
            }
          }
    }
}
