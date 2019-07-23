pipeline {
  agent {
    docker {
      image 'nginx'
    }
    }
  }

  stage {
    stage ('Testing') {
      steps {
        sh 'docker run -p 8082:80 -d -v /home/stagiaire/docker-nginx-2/html:/usr/share/nginx/html nginx
'
      }
    }
  }
