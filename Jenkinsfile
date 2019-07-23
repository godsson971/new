pipeline {
    agent { docker 'nginx' }
    stages {
        stage('Test') {
            steps {
                sh('chmod +x docker.sh')
                sh('./docker.sh')

            }
        }
    }
}
