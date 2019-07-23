pipeline {
    agent { docker 'nginx:preprod' } 
    stages {
        stage('Test1') {
            steps {
                sh 'docker stats preprod'
            }
        }
    }
}
