pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Test') {
            steps {
                sh 'test -f Index.html'
            }
        }

        stage('Deploy') {
            steps {
                sh 'cp Index.html /var/www/html/index.html'
            }
        }
    }
}
