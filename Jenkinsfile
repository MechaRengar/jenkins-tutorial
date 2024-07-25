pipeline {
    agent any

    stages {
        stage('Pull Code') {
            steps {
                // Pull the latest code from the repository
                git 'https://oauth2@github.com/MechaRengar/node-express-boilerplate.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                // Install npm dependencies
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                // Run the test script
                sh 'npm run test'
            }
        }
    }
}
