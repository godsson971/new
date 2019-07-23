pipeline {
    agent { docker 'nginx' }
    stages {
        stage('Test') {
            steps {
                                                             
                sh('bash -x ./docker.sh')
                
            }
        }
    }
}
