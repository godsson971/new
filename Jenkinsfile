pipeline {
    agent { docker 'nginx' }
    stages {
        stage('Test') {
            steps {
                sh('docker run -p 8082:80 -d nginx')

            }
        }
    }
}
