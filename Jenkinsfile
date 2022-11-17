#!groovy

def tagName = ""
def folderName = ""
pipeline {
    agent any 
    stages {
        stage('Get Dependencies') {
            steps {
                echo 'Get Dependencies..'
                npm install -D 
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
                npm run build
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