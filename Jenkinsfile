pipeline {
    agent {
        docker { image 'node:14-alpine' }
    }
    
    environment {
        DOTNET_CLI_HOME = '/tmp'
    }

    stages {
        stage('Build') {
            steps {
                dotnet build
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