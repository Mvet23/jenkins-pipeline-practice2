pipeline {
    agent any
    stages {
        stage('clone') {
            steps {
                sh 'echo "Cloning repository..."'
                // Add git clone command if needed
                // git url: 'https://github.com/utrains/nodeLogin.git', branch: 'main'
            }
        }
        stage('test') {
            steps {
                sh 'echo "Running tests..."'
            }
        }
        stage('createfile') {
            steps {
                sh 'touch text-${BUILD_ID}.txt'
            }
        }
    }
}