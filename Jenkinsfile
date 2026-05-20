pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/MayankBansal07/devops-deployment-dashboard.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Build Successful'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                sudo cp -r * /var/www/html/
                '''
            }
        }
    }
}