pipeline {
    agent { docker 'nginx' }
    stages {
        stage('Test') {
            steps {
                sh('mkdir /tmp/test-jenkins')
                sh('touch /tmp/test-jenkins/docker.sh')
                sh('echo "toto" > /tmp/test-jenkins/docker.sh')
               
            }
        }
    }
}
