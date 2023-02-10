pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building.'
                sh 'dotnet build && cd DotnetTemplate.Web && npm install && npm run build && npm run lint'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'dotnet test && cd DotnetTemplate.Web && npm t'
            }
        }
        
    }
}