pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'make -C main' 
            }    
        }    

        stage('Test') {
            steps {
                sh './main/hello_exec'
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
