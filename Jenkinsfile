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
                bat '''
                    if not exist C:\\inetpub\\wwwroot mkdir C:\\inetpub\\wwwroot
                    copy /Y index.html C:\\inetpub\\wwwroot\\
                '''
            }
        }
    }
}