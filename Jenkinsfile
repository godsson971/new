pipeline {
    agent { docker 'nginx' }
    stages {
        stage('Test') {
            steps {
                sh('/usr/bin/docker --version')

            }
        }
    }
}
