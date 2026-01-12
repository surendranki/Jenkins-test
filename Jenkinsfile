pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/surendranki/jenkins-test.git'
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Building application..."'
            }
        }

        stage('Test') {
            steps {
                sh './test.sh'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "Deploying application..."'
            }
        }
    }
}
