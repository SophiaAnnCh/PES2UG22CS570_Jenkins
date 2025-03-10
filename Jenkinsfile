pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'g++ hello_pes2ug22cs570.cpp -o PES2UG22CS570-1'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Testing the project...'
                sh './PES2UG22CS570-1'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
