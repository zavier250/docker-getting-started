pipeline {
    agent any
    
    stages {
        
//         stage('Switch to root') {
//             steps {
//                 sh 'sudo -i'
//             }
//         }
        stage('Build Docker image') {
            steps {
                sh 'docker build -t docker-getting-started .'
            }
        }

        stage('Run Docker Container') {
            steps {
                sh 'docker run -dp 3000:3000 docker-getting-started'
            }
          }
    }
}
