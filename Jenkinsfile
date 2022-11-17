#!groovy

def tagName = ""
def folderName = ""
pipeline {
    agent any 
    stages {
        stage('Get Dependencies') {
            steps {
                echo 'Get Dependencies..'
                sh 'node -v' 
            }
        }
        stage('Get Dependencies') {
            steps {
                echo 'Get Dependencies..'
                sh 'npm install -D' 
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'npm run build'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}