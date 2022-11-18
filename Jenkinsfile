#!groovy

def tagName = ""
def folderName = ""
pipeline {
    agent any 
    tools { nodejs "node"}
    stages {
        stage('Get Dependencies') {
            steps {
                npm install
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