        
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout source code from version control
                checkout scm
            }
        }

        stage('Build') {
            steps {
                // Install dependencies and build React app
                sh 'apt-get install npm'
                sh 'npm install'
                sh 'npm run build'
            }
        }
}
}
