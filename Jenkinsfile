pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Deploy Application') {
            steps {
                // Windows batch command to copy index.html to your local web directory
                bat 'copy /Y index.html C:\\inetpub\\wwwroot\\'
            }
        }
    }
}