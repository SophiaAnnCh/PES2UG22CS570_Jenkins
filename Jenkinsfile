pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ main/hello.cpp -o main/hello'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './main/hello'
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment Stage: No actual deployment in this lab.'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed!'
        }
    }
}
