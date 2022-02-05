pipeline {
    stages {      

        stage('Build Docker image') {
            def built_img = ''
            built_img = docker.build('./')
            built_img.tag('docker-getting-started')
        }

        stage('Run Docker Container') {
          sh 'docker run -dp 3000:3000 docker-getting-started'
        }
    }
}
