pipeline {
    agent any

    environment {
        PATH = "/usr/local/bin:$PATH" // Add Yarn installation directory to PATH
    }

    stages {
        stage('Install Homebrew') {
            steps {
                sh '/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"'
            }
        }

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
