#!groovy

def tagName = ""
def folderName = ""
pipeline {
    agent any 
    tools { nodejs "node"}
    stages {
        stage('Permision') {
            steps {
                sh('ls -la ..')
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
                sh('npm install')
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