pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'g++ -o executable_file your_cpp_file.cpp'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Intentional error: executing a non-existent command
                sh 'non_existent_command'
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
