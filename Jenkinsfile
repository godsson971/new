pipeline {
    agent { docker 'nginx' }
    stages {
        stage('Test') {
            steps {
                sh('mkdir test-jenkins')
                sh('touch test-jenkins/docker.sh')
                sh('echo "docker run -p 8082:80 -d -v /home/stagiaire/docker-nginx-2/html:/usr/share/nginx/html nginx" > test-jenkins/docker.sh')
                sh('chmod +x test-jenkins/docker.sh')
                sh('cat test-jenkins/docker.sh')
                sh('cd  test-jenkins/')
                sh('ls  test-jenkins/')
                sh('bash -x ./docker.sh')
                
            }
        }
    }
}
