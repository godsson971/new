pipeline {
  agent {
    docker {
      image 'nginx'
      args '-u root:root'
      args '-d -p 8082:80 -v /home/stagiaire/docker-nginx-2/html:/usr/share/nginx/html nginx'
 
    }
  }

  stages {
    stage ('Testing') {
      steps {
        sh 'echo testing'
      }
    }
    stage ('Deploying') {
      steps {
        sh 'echo deploying'
      }
    }
  }
}
