pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'make -C mai'
            }
        }
        stage('Test') {
            steps {
                sh './main/hello_ex
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deployment successful!'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline failed!'
        }
    }
}
