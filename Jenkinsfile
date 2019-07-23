pipeline {
  agent none
  stages {
    stage('Nginx Install') {
      agent {
        docker {
          image 'nginx'
        }
      }
      steps {
        sh 'nginx clean install'
      }
    }
    stage('Docker Lauch') {
      agent any
      steps {
        sh 'docker run -p 8082:80 -d -v /home/stagiaire/docker-nginx-2/html:/usr/share/nginx/html nginx'

      }
    }
