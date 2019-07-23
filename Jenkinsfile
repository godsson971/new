pipeline {
    agent {
        docker { image 'node:nginx }
    }
    stages {
        stage('Test1') {
            steps {
                sh 'node --version'
            }
        }
    }
}
