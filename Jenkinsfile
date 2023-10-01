pipeline {
    agent any

    environment {
        PATH = "/usr/local/bin:$PATH" // Add Yarn installation directory to PATH
    }

    stages {
        stage('Check Yarn Version') {
            steps {
                sh 'brew install yarn && yarn --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'yarn install'
            }
        }
    }
}
