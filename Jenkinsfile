pipeline {
 agent any
 stages {
 stage('Build') {
 steps {
 sh 'g++ -o PES2UG20CS370-1 ./main/he.cpp'
 echo 'Building successful'
 }
 }
 stage('Test') {
 steps {
 sh 'PES2UG20CS370'
 echo 'Testing successful'
 }
 }
 stage('Deploy') {
 steps {
 echo 'Deploying successful'
 }
 }
 }
 post {
 failure {
 echo 'Pipeline failed'
 }
 }
}

