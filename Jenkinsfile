pipeline {
    agent any
    stages {
         stage('Checkout') {
            steps {
                sh 'git clone "https://github.com/Jagruthi111/Container.git"'
            }
        }
      stages {
        stage('Build Docker Image') {
            steps {
                script {
                    docker.build("terraform-img:1.0", "-f dockerfile .")
                }
            }
        }
    }
}
