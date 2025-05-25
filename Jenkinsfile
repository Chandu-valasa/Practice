pipeline {
    agent any
    stages {
        stage('checkout') {
            steps {
                git url: 'https://github.com/Chandu-valasa/Practice.git', branch: 'master'
                // Add your build commands here
            }
        }
        stage('build') {
            steps {
                script {
                    sh 'ls -ltr'
                    sh 'python3 simplr.py'
                    }
                // Add your test commands here
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add your deployment commands here
            }
        }
    }
}