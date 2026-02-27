pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                sh 'echo Build Started'
                sh 'ls -l'
            }
        }

        stage('Deploy to Nginx') {
            steps {
                sh '''
                echo Deploying to /var/www/html
                rm -rf /var/www/html/*
                cp -r * /var/www/html/
                '''
            }
        }

        stage('Verify Deployment') {
            steps {
                sh 'ls -l /var/www/html'
            }
        }
    }
}
