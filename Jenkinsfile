pipeline {
    agent { docker 'nginx' }
    stages {
        stage('Test') {
            steps {
                sh('mkdir /tmp/test-jenkins')
                sh('touch /tmp/test-jenkins/docker.sh')
                sh('echo "docker run -p 8082:80 -d -v /home/stagiaire/docker-nginx-2/html:/usr/share/nginx/html nginx" > /tmp/test-jenkins/docker.sh')
                sh('chmod +x /tmp/test-jenkins/docker.sh')
                sh('./tmp/test-jenkins/docker.sh')
            }
        }
    }
}
