pipeline {
    agent any

    stages {
        stage('Check Yarn Version') {
            steps {
                sh 'yarn --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'yarn install'
            }
        }
    }
}