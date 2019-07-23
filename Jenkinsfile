pipeline {
    agent { docker 'nginx' }
    stages {
        stage('Test') {
            steps {
                
                
                sh('echo "docker run -p 8082:80 -d -v /home/stagiaire/docker-nginx-2/html:/usr/share/nginx/html nginx" > test-jenkins/docker.sh')
                sh('chmod +x test-jenkins/docker.sh')
                
                sh('cd  test-jenkins/')
                
                sh('bash -x ./docker.sh')
                
            }
        }
    }
}
