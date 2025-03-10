pipeline {
    agent any
    environment {
        FILE_NAME = "text-${BUILD_ID}.txt"
    }
    stages {
        stage('clone') {
            steps {
                sh 'echo "Cloning repository..."'
                //git url: 'https://github.com/utrains/nodeLogin.git', branch: 'main'
            }
        }
        stage('test') {
            steps {
                sh 'echo "Running tests..."'
            }
        }
        stage('createfile') {
            steps {
                sh "touch ${FILE_NAME}"
            }
        }
    }
    post {
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}