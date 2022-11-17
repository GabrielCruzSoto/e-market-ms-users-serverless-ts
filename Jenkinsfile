#!groovy

def tagName = ""
def folderName = ""
pipeline {
    agent any 
    stages {
        stage('version node') {
            steps {
                
                echo 'pwd'
                sh 'pwd'
                echo 'PATH'
                sh 'echo $PATH'
                echo 'node -version'
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