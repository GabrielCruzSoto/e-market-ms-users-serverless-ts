#!groovy

def tagName = ""
def folderName = ""
pipeline {
    agent any 
    tools { nodejs "node"}
    stages {
        stage('Get Dependencies') {
            steps {
                sh 'npm install'
                echo 'Get Dependencies..'
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
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