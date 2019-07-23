pipeline {
    agent {
        docker { image 'nginx:latest' }
    }
    stages {
        stage('Test1') {
            steps {
                sh 'docker run --name preprod -p 8082:80 -d -v /home/stagiaire/docker-nginx-2/html:/usr/share/nginx/html nginx'
            }
        }
    }
}
