pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'make -C nonexistent_dir' 
            }    
        }    

        stage('Test') {
            steps {
                sh './main/hello_ex
            }
        }
        stage('Deploy') {
            steps {
                echooo 'Deployment successful!'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline failed!'
        }
    }
}
