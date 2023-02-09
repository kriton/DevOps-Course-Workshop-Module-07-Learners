pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'echo pwd'
                sh 'dotnet build'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'dotnet test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}