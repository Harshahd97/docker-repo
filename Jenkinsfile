pipeline {
    agent { dockerfile true }
    stages {
        stage('Test') {
            steps {
                script {
                    // Build the Docker image
                    docker.build("my-terraform-image")

                    // Run the Docker container
                    docker.image("my-terraform-image").inside {
                        sh 'terraform --version'
                    }
                }
            }
        }
    }
}
