pipeline {
    agent { docker 'nginx' }
    stages {
        stage('Test') {
            steps {
                sh('build -t .')

            }
        }
    }
}
