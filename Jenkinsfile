pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'g++ -o executable_file main.cpp'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh './executable_file'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add commands to deploy your project
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
