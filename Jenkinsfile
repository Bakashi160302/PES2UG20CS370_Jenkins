pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES2UG20CS370-1 PES2UG20CS370-1.cpp'
            }
        }
        stage('Test') {
            steps {
                sh './PES2UG20CS370-1'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deployment successful"'
            }
        }
    }
    
    post {
        failure {
            echo "Pipeline failed"
        }
    }
}
