pipeline {
    agent { docker 'nginx' }
    stages {
        stage('Test') {
            steps {
                sh('/var/lib/jenkins/workspace/testdockerpipeline/docker.sh')
               
            }
        }
    }
}
