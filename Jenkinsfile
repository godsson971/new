pipeline {
    agent { docker 'preprod' } 
    stages {
        stage('Test1') {
            steps {
                sh 'docker stats preprod'
            }
        }
    }
}
