pipeline {
    agent {
        docker {
            dockerfile true
            // Optionally, you can specify additional parameters like args
            // args '-v /tmp:/tmp'
        }
    }
    stages {
        stage('Test') {
            steps {
                sh 'terraform --version'
            }
        }
    }
}
