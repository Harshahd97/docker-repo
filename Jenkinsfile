pipeline {
    agent { dockerfile true }
    stages {
        stage('Test') {
            steps {
                sh 'sudo chmod 777 /var/run/docker.sock'
                sh 'terraform --version'
                
            }
        }
    }
}
