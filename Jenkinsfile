pipeline {
    agent {
        docker { image 'nginx:latest' }
    }
    stages {
        stage('Test1') {
            steps {
                sh 'docker images nginx'
            }
        }
    }
}
