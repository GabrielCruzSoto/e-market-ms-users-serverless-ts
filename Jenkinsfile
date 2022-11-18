#!groovy

def tagName = ""
def folderName = ""
pipeline {
    agent any 
    tools { nodejs "node"}
    stages {
        stage('Get Dependencies') {
            steps {
                sh('npm install')
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
                sh('npm run build')
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