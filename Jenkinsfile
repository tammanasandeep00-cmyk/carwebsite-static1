
pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                echo 'Cloning repository...'
            }
        }

        stage('Build') {
            steps {
                sh 'echo Build Started'
                sh 'ls -l'
            }
        }

        stage('Test') {
            steps {
                sh 'echo Testing Static Website'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo Deployment Stage'
            }
        }
    }
}
