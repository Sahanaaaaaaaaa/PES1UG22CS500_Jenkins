pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'make -C nonexistent_dir' // This directory doesn't exist
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
