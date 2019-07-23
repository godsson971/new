pipeline {
    agent {
        docker { restart 'preprod' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'docker ps'
            }
        }
    }
}
